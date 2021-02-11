# Next.css Reset Module

Reset CSS Module is part of Next.css framework. This module resets default CSS styles for your Next.css project.
You can use in all modern websites with module bundlers, like webpack, rollup, parcel.

## How to Install

You can install with **npm** or **yarn** package managers.

```
npm i @nextcss/reset
yarn add @nextcss/reset
```

## How to use

Simple import to your project, this module contains only element selector rules.

```
import '@nextcss/reset';
```

## Why you should use

Some HTML Elements has a default style in browsers and some HTML Elements styled different in each browsers. This module will resets this styles.

## Features

- Reset most common HTML Element styles
- Reset Outline and Tap highlighting
- Reset Drag and Drop
- Reset Pull to Refresh and Scroll Chaining
- Reset Pinch Zoom and Touch Gestures
- Set Box Sizing
- Set System Font Stack with `14px` font size and `1.4` line height

## What's included - TL;DR

On every HTML Elements: set `border-box` as default `box-sizing`, disable `Drag and Drop` feature and reset `outline`.

```css
*,
:before,
:after {
  box-sizing: border-box;
  -webkit-user-drag: none;
  outline: none;
}
```

Set default `font-size` to `14px`, disable `Tap highlighting` for mobile devices, enable `Smooth font rendering`, disable `Text size increase algorithm` for apple devices.

```css
html {
  font-size: 14px;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-smoothing: antialiased;
  -webkit-text-size-adjust: 100%;
}
```

Disable `pinch zoom` and other `touch gestures`, disable `pull to refresh`, `rubber banding` and `scroll chaining` features, set `max-width` on `body` as `100 viewport width`, reset default `margin`, set default `line-height` and `Systen Font Stack`

```css
body {
  touch-action: pan-x pan-y;
  overscroll-behavior: none;
  max-width: 100vw;
  margin: 0;
  line-height: 1.4;
  font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, 'Noto Sans', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
}
```

Reset default `margin` and `font` properties on Headings and Paragraph.

```css
h1,
h2,
h3,
h4,
h5,
h6,
p {
  margin: 0;
  font: inherit;
}
```

Reset `color` and `text-decoration` on links.

```css
a {
  color: inherit;
  text-decoration: none;
}
```

Limit image `width` and reset `border`.

```css
img {
  max-width: 100%;
  height: auto;
  border: none;
}
```

Reset `border`, `shadow`, `font` and set `font-size` to `16px` on common input elements. `16px` font size avoid resizing `viewport` on apple devices.

```css
input,
textarea,
select {
  font: inherit;
  font-size: 16px;
  border: 1px solid;
  border-radius: 0;
  background-clip: padding-box;
}

fieldset {
  border: 1px solid;
}
```

Reset `margin`, `padding` and `list-style` on lists.

```css
ul,
ol {
  margin: 0;
  padding: 0;
  list-style-type: none;
}
```

Reset `border` of horizonal rule

```css
hr {
  border: none;
  border-bottom: 1px solid;
}
```

Reset `table` border and table head `font-weight`

```css
table {
  border-spacing: 0;
  border-collapse: collapse;
}

th {
  font-weight: inherit;
}
```

Reset iframe `border`

```css
iframe {
  border: 0;
}
```

Reset `margin` and `padding` on common HTML Elements

```css
menu {
  margin: 0;
  padding: 0;
}

form,
figure,
pre,
blockquote,
dl,
dd {
  margin: 0;
}
```

Reset `font` on `adrress` tag

```css
address {
  font: inherit;
}
```

## License

MIT License. Copyright (c) 2021 Zsolt Tovis
