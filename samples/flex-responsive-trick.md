# Using flex for making responsive websites

Flex can be pretty handy for making responsive websites. The trick is to combine it with media-query.

Say we have a [page with a sidebar](https://codepen.io/faltoo/pen/dyMxpBp). The css will be:

```css
.page {
  display: flex;
  flex-direction: row;
}
```

![Sidebar Layout](../assets/sidebar-layout.png)

For mobiles, we can change the `flex-direction` to `column`.

We can use media queries to make such changes based on device width. A good way to proceed is to **write the css for mobile first**. We should then use media queries for desktop interfaces.

The complete CSS for the above will be:

```css
/* We start with the CSS for mobile */
.page {
  display: flex;
  flex-direction: column;
}

/* And then add media queries for larger devices */
@media (min-width: 768px) {
  .page {
    flex-direction: row;
  }
}
```

This is called **mobile-first approach**.
