# Week 4

During week 1 and 2, we saw that deployment is hard. We need to do multiple things to deploy a website:

- handle python versions and virtual env
- install nginx
- install MySQL
- install gunicorn

## Task: Migrate the website with data to AWS

Try to migrate your full website to AWS.

*Like we need to format our computers once in a while, similarly we need to change our servers once in a while.*

We often need to change the servers because of:
- Better hardware on some other host.
- Need more resources (more ram or CPU). While 1GB ram might be cheaper on DigitalOcean, 16GB ram might be better on AWS.

On Screener, would have migrated servers over 7 times. From shared hosting to VPS to larger VPS to AWS.

## Next task

Think about the problems faced. What took most of the time during migration. Explore options to automate these tasks.

Look at:
- Ansible
- Chef
- Any other solutions?

## Include configuration for NGINX and MySQL inside codebase

Can we have a solution which allows us to version control the configs for services like NGINX, MySQL etc?

## Look at Docker

What if we can write a shell script to automate all these stuff? And include that shell script in our source code? That is exactly what Docker does.
