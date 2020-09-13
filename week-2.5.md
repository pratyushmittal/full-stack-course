# Week 2.5 - JS stuff

You have a basic website ready. You can push new updates in seconds. Its time to add new features now.

The plain text posts are not very pretty. We should be able to add links and basic styling such as bold text.

## Tasks

### Better posts with rich text content *~3 days*

- Add ability to insert links and bold text in the posts.
- Sanitize the input to ensure user can't insert malicious html content such as javascript.
- Sanitize the input at server level too.

## Resources

- Docs on [`contenteditable`](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Editable_content)
- About [XSS](https://www.google.com/about/appsecurity/learning/xss/) attacks with doable examples
- [XSS](https://docs.djangoproject.com/en/3.1/topics/security/#cross-site-scripting-xss-protection) protection in Django
- Try to avoid using any JS library and write your own component for rich text editing. Use [Trix](https://trix-editor.org) only if it becomes too hard to do it yourself.
- [Bleach](https://bleach.readthedocs.io/en/latest/)


## Food for thought

- At what levels should we sanitize the content? Should we sanitize the output too?
