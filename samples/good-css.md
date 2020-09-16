# Tips for sane CSS

## Use functional CSS instead of modular

Bad:
```css
.documents-holder {
    display: flex;
    margin: -8px;
}

.documents {
    margin: 8px;
}
```

Good:
```css
.flex {
    display: flex;
}

.flex.flex-gap-16 {
    margin: -8px;
}

.flex.flex-gap-16 > * {
    margin: 8px;
}
```

## Use properties as names

Bad: `.shadowed`
Good: `.box-shadow`

Bad: `.rounded-medium`
Good: `.radius-6`

## Style attributes are cool

There will be more number of padding and margin needs than you think.

```
padding: 10px 14px;
padding: 8px 14px;
padding: 8px;
padding: 16px;
padding: 4px 6px;
```

It is better to set them at element level. Use utility classes for padding or margin only when you need media queries.

## Prevent from using CSS variables in style elements

While padding and margins are good at element style level, colors are better at utility level.

Bad: `<p style="font-weight: 500; color: var(--ink-900);">...</p>`
Good: `<p class="font-weight-500 ink-900"></p>`
