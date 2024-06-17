# Translating simple-card UI

### Key learnings:

- aria-hidden="true" so that screen reader can ignore the arrow as its a decorative thing that does not effect the UX.
- `.cta`(call to action) normally used as lingo for links in web dev
- `box-sizing: border-box` without this the `height` & `width` only include the area of the element and not `padding` or `border`. However when we use this it enables for the `padding`, `border` and `area` of the element to be included within the `height` and `width`. Making layout calculations more predictible.
- to work out `em` when `font-size` of parent element is `16px`: `8px` into `em` = 8 / 16 = `0.5em`
- `rem` always looks at the root element `font-size`
- `em` will look at the nearest parent font-size, if none has been set, it will look at the root `html` `font-size`

The below `css` code makes it so that `1em` or `1rem` will equal `10px` instead of `16px`.

- 62.5% x 16 = 10 or 0.625 x 16 = 10

```css
html {
  font-size: 62.5%;
}
```

# Design

![Figma design for - simple card](./assets/simple-card.png)
