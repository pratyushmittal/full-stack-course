# Week 1

The most important part of starting is to be live as soon as possible. In week 1 we will focus on getting our website live. Getting the most minimum working.

We should focus only on minimum needed for a website. Minimum means that we can focus on design later. Minimum means having a production server.

## Tasks

### Preparing the minimum viable product (MVP) *~3 days*

- Create a Django project for a Twitter like collaborative blog. Anyone can register and write a post. A post will have a title and text content.
- There will be a home page, login page and registration page.
- Home page will show latest posts in decreasing order. It will have pagination.
- Write CSS as you need. Don't focus on looks to much. Get the minimum working. **DON'T use a CSS framework such as Bootstrap.

### Getting it live *~2 days*

- Create a remote server. Use Amazon EC2's free tier or DigitalOcean's $5 droplet.
- Install needed dependencies. Probably, MySQL, nginx and gunicorn.
- Copy the code to remote server. Use FTP or whatever you are comfortable with.
- Follow Django's deployment guide to deploy.


## Resources

- Follow 6 steps [Django Tutorial](https://docs.djangoproject.com/en/3.1/intro/tutorial01/) with the above task in mind.
- [Django's documentation](https://docs.djangoproject.com/en/3.1/) is super awesome. Refer it whenever you read about a new Django function or API.
- Use [DevDocs](https://devdocs.io) or [Dash](https://kapeli.com/dash) for easy reference to documentation. Keep it always open.
- DigitalOcean is easier to get started than EC2.
- Learn [basics of `vim`](https://github.com/snori74/linuxupskillchallenge/blob/d0f12c3c2cf29e6860e918516cc2c5cc4b87eab1/06.md) for easier text editing on remote server.
- Follow [Django's deployment guide](https://docs.djangoproject.com/en/3.1/howto/deployment/wsgi/gunicorn/) using Gunicorn and nginx. Skip virtualenv on production for now.
- Initially the website will just not start. Keep persisting. Focus on `nginx` logs and `gunicorn` logs to trace the reasons.


## Rules

- I will **not** provide any solution.
- You need to develop a habit of searching good content and referring the documentation.
- I *will* review the *working* code if you want. Add me to your repository and ask me to look through it. I will provide a positive feedback.
