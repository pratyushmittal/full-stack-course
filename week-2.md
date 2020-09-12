# Week 2

Congrats your app is running now! But it is not fun to access website using IP. So our week 2 task is to get domain and make incremental updates easier.

## Tasks

### Easier deployment *~1 day*
- Get a domain name and configure DNS
- [Setup remote-repository to push updates](https://gist.github.com/noelboss/3fe13927025b89757f8fb12e9066f2fa) to website by simply running "git push live"
- Extend the above trick to [automate Django deployment](./samples/post-receive-django.md) too.
- Bonus: [Split Django settings](https://simpleisbetterthancomplex.com/tips/2017/07/03/django-tip-20-working-with-multiple-settings-modules.html) into different setting files for local, testing and remote server.

### Better UI *~2 days*
- Add [basic styling](https://jgthms.com/web-design-in-4-minutes/) to your website
- Colors and Typography make 90% of the design. They are what make your design unique. Go through the resources below to learn about them.
- Customize forms and buttons for your own unique look. Refer to [Skeleton CSS source code](https://github.com/dhg/Skeleton/blob/master/css/skeleton.css) to see how they customized the forms and buttons. See only the forms and buttons section in the source code.
- Try to create buttons similar to ones used on [Stripe's website](https://stripe.com/docs).

### Better posts with rich text content *~3 days*

Move to [Week 2.5](./week-2.5.md).


## Resources
- I recommend Google Domains because they provide free email forwarding and better privacy.
- Refer [MDN docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) whenever you use a new CSS property.
- **Don't use w3schools**. You won't *learn* anything if you use W3Schools because they don't explain the concepts.
- Add MDN docs to your doc reference software such as Dash or DevDocs.
- [Choosing Colors](https://refactoringui.com/previews/building-your-color-palette/): Very good lesson on how to think about colors.
- [Color in UI Design](https://learnui.design/blog/color-in-ui-design-a-practical-framework.html): Wonderful post on how to choose good colors.
- [UI Typography by Apple](https://developer.apple.com/videos/play/wwdc2020/10175/): Video explains why we need different font settings for different sizes. It will explain how and why to choose different `line-height` and `letter-spacing` for different font sizes.
- [Monica.css](https://meowni.ca/posts/monica-dot-css/): Beautiful post on why we don't need a CSS framework today.
- [CSS Variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties): CSS variables are one of the most useful things in CSS.


## Self Evaluation
- Why do we need normalize.css?
- What's the deference between css reset and css normalization?
- What does `margin: 0 auto` do in css?