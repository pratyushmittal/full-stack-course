# Week 3

Nice! We can write small blog posts now. And we can quickly deploy the updates.

But blog posts are not very useful without images. Now we will add ability to upload images.

----

## Task 1
*~3 days*

### Allow images uploads in posts

Allow Basecamp type image uploading. A person can drop an image and it uploads. Then insert it in the rich text editor. Can move to [Trix](https://trix-editor.org) for now.

### Resources
- [Media files in Django](https://docs.djangoproject.com/en/3.1/topics/files/): It tells how to save and link to user uploaded media files. We might not need to "use files in models" but use it to create a simple upload API.
- [Tips for writing good functions](./samples/functions.md): Few tips on writing good functional code.
- [Trix Rich Text Editor](https://github.com/basecamp/trix): Replace our own `contenteditable` component with Trix. Trix already has JS support for handling image drops.
- [Example of image uploads](https://trix-editor.org/js/attachments.js): We will create our own Django API instead of using Cloudfront in example.

----

## Task 2
*~3 days*

- Bottom bar on mobiles
- Fixed header
- Two column design
- Same row with name on left and date on right

### Resources
- [Golden ratio]
- [Display]
- [CSS Tricks - Flex Cheatsheet]
- [Mastering Flex]
- [Grid snap-columns]
- [Functional CSS]
