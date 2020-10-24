# Week 2

Congrats your app is running now! But it is not fun to access website using IP. So our week 2 task is to get domain and make incremental updates easier.

## Tasks

### Easier deployment *~1 day*
- Get a domain name and configure DNS
- [Setup remote-repository to push updates](https://gist.github.com/noelboss/3fe13927025b89757f8fb12e9066f2fa) to website by simply running "git push live"
- Extend the above trick to [automate Django deployment](./samples/post-receive-django.md) too.
- Bonus: [Split Django settings](https://simpleisbetterthancomplex.com/tips/2017/07/03/django-tip-20-working-with-multiple-settings-modules.html) into different setting files for local, testing and remote server.

### Better UI *~2 days*
- Add the basic styling to your website: https://jgthms.com/web-design-in-4-minutes/
- Most of the design stuff is just font, colors and typography. Let's get them done.
- For fonts, choose one from Google Fonts.
- For colors, read this chapter: https://refactoringui.com/previews/building-your-color-palette/
- In the end, try to make a custom button. Try to make similar to on on Stripe's website: https://stripe.com/docs
- Next is to customize forms. Forms are just labels and inputs. By default the labels are shown inline. Let's show them in new line using `display: block` on `label`. For text input boxes, keep a padding of `8px 12px` and add other styling you like.


### Better posts with rich text content *~3 days*

Move to [Week 2.5](./week-2.5.md).


## Resources
- I recommend Google Domains because they provide free email forwarding and better privacy.
- Refer [MDN docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) whenever you use a new CSS property.
- **Don't use w3schools**. You won't *learn* anything if you use W3Schools because they don't explain the concepts.
- Add MDN docs to your doc reference software such as Dash or DevDocs.
- [Color in UI Design](https://learnui.design/blog/color-in-ui-design-a-practical-framework.html): Another wonderful post on how to choose good colors.
- [Monica.css](https://meowni.ca/posts/monica-dot-css/): Beautiful post on why we don't need a CSS framework today.
- [CSS Variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties): CSS variables are one of the most useful things in CSS.


## Self Evaluation
- What does `margin: 0 auto` do in css?
- Read a bit about normalized CSS and why do we need it.