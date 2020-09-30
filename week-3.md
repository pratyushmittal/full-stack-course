# Week 3

Nice! We can write small blog posts now. And we can quickly deploy the updates.

Starting using your project as a daily journal. Post updates about daily progress. Using your project yourself will make it usable.

----

## Task 1
*~3 days*

### Allow images uploads in posts

You will ultimately use the blog posts only if it is easy to upload pictures. Allow Basecamp type image uploading. Add ability to drop an image and it uploads and inserts in the rich text editor. Can move to [Trix](https://trix-editor.org) for now.

### Resources
- [Media files in Django](https://docs.djangoproject.com/en/3.1/topics/files/): It tells how to save and link to user uploaded media files. We might not need to "use files in models" but use it to create a simple upload API.
- [Tips for writing good functions](./samples/functions.md): Few tips on writing good functional code.
- [Trix Rich Text Editor](https://github.com/basecamp/trix): Replace our own `contenteditable` component with Trix. Trix already has JS support for handling image drops.
- [Example of image uploads](https://trix-editor.org/js/attachments.js): We will create our own Django API instead of using Cloudfront in example.

----

## Task 2
*~3 days*

![Desktop prototype](./assets/desktop.png)

Let's learn some frontend techniques now. You might want to brush up your [CSS basics][] if you are new to it.

Before we make changes on our 


### Add options to posts and improve mobile interface
Target:
<!-- media-query: show on mobile, flex-column -->
<!-- stacking: dropdown menu -->
flex: menu-bars, navigation
flex-wrap: tags, inside menu
flex-gutter: wherever flex-wrap
flex-columns for mobile trick
auto-fill grid: archives or authors page

- Bottom bar on mobiles
- Options menu on posts
- Fixed header
- Two column design
- Same row with name on left and date on right

### Resources
- [CSS Basics]: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics
- [Position]: How position works in CSS
- [CSS Tricks - Flex Cheatsheet]
- [Mastering Flex]
- [Grid](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids): Grid is powerful but complex. Read this one completely and you will master most of its techniques.
- [Functional CSS]
