# Week 2.5 - JS stuff

You have a basic website ready. You can push new updates in seconds. Its time to add new features now.

The plain text posts are not very pretty. We should be able to add links and basic styling such as bold text.

## Tasks

### Better posts with rich text content *~3 days*

- Add ability to insert links and emphasis in the posts.
- Sanitize the input to ensure user can't insert malicious html content such as javascript.
- Sanitize the input at server level too.

## Resources

- `contenteditable`
- XSS
- [Bleach]()
- Try to avoid using any JS library and write your own component for rich text editing. Use [Trix]() only if it becomes too hard to do it yourself.

## Food for thought

- At what levels should we sanitize the content? Should we sanitize the output too?
