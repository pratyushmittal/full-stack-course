# Run migrations on post-receive

The [post-receive hook trick](https://gist.github.com/noelboss/3fe13927025b89757f8fb12e9066f2fa) checkouts the latest code. It saves us from manually copying files over FTP.

We still need to do various things to see the latest code changes:
- run migrations
- run collectstatic
- restart gunicorn server
- any other step if needed

These additional steps keep changing over the life of the code.

A good way to automate these too is to add a `bash` script for these jobs.

We can change our post-receive hook to run this script after checking out the new code.

I use something like this in the `post-receive` hook.

```bash
#!/bin/bash

PROJECT=/home/ubuntu/{project}
BRANCH=master

echo "Project is $PROJECT with branch $BRANCH"

# exit if anything fails
set -e

echo "Checking out new code"
mkdir -p $PROJECT
git --work-tree=$PROJECT checkout $BRANCH -f

echo "Running post-receive"
cd $PROJECT
bash deploy.sh
```

Then you can create `deploy.sh` to run `makemigrations` and other commands. This `deploy.sh` can now be the part of your source code.

A sample `deploy.sh` can be something like:

```bash
#!/bin/bash

# On git push, this script will run automatically on server

set -e  # exit if anything fails

echo "Collecting Static files"
python manage.py collectstatic --noinput --settings=project.settings.production

echo "Running migrations"
$RUN python manage.py migrate --settings=project.settings.production

# Add other commands as needed
```
