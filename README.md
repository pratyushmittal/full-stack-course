# What is this about?

This course will give you skills to create a full website. From scratch to deployment.

Being a "full-stack" engineer requires multiple skills. It can be overwhelming to think of all of them. **This guided provides a step-by-step guide to learn and practice those skills.**

By the end of the course, you will probably be able to:

- create a Django application
- create remote servers 
- use ssh
- use nginx
- deploy app using "git push"
- use crons
- use SSL and LetsEncrypt
- configure domain names (DNS records)

- Write advanced Javascript
- Write advanced CSS

- create virtual machines (containers) using Docker
- run multiple containers together using Docker Compose

- Migrate servers


## Overview

It assumes that a person reading this guide already has a basic knowledge of:

- html
- css
- git
- know how websites work


## Rules

- I will **not provide** any solutions.
- You need to develop a habit of searching good content and referring the documentation.
- Sleep over the problem when you get stuck. Sometimes the solutions come at night or next day. Develop this instinct.
- Ask on StackOverflow or IRC channels if you get stuck.
- I **will** review the *working* code if you want.


### Course outline

- Create a very simple blog: something like Twitter
    - anyone can register and post in plain text
    - show all posts in decreasing order
- push it to production
    - setup a remote server
    - copy code to remote server
    - install MySQL
    - install nginx
    - setup gunicorn
- add a domain name
    - purchase a domain name
    - setup DNS records
- setup git-push
    - add repository
    - add post-receive hook
- improve design
    - normalize.css
    - mobile first and minimal CSS needed
    - use external font
    - style buttons and form
- handle rich text
    - use contenteditable and Javascript
    - use Bleach to sanitize content
- handle image uploads
    - ajax and drop even handlers
- re-deploy everything
    - understand need for server automation
    - write Dockerfile
    - write docker-compose.yml
- monitoring and routine tasks
    - crons for error logs
    - include crons in source code
    - cron to create a backup everyday
- make the design *smart*
    - show more using css
    - show tooltips
    - three column design:
        - toc
        - content
        - footnotes
- change the web-host
    - deploy a new server
    - put website on maintenance
    - create a backup
    - restore backup on new web-host
    - update DNS records
