---
layout: post
title: 学习Flexbox
date: 2022-01-04 21:28 +0800
toc: true
tags: 
  - CSS
  - 背
---
Flexbox is a one-dimensional layout method for arranging items in rows or columns.

Note: Flexbox layout is most appropriate to the components of an application, and small-scale layouts, while the Grid layout is intended for larger scale layouts.

## Flexbox Properties

### Properties for the Parent: (flex container)

display

```css
display: flex; /* or inline-flex */
```

flex-direction
```css
flex-direction: row | row-reverse | column | column-reverse;
```

flex-wrap
```css
flex-wrap: nowrap | wrap | wrap-reverse;
```

flex-flow: This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.
```css
flex-flow: column wrap;
```

justify-content
```css
justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
```

align-items
```css
align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
```

align-content
```css
align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
```

gap, row-gap, column-gap
```css
gap: 10px 20px; /* row-gap column gap */
```

### Properties for the Children (flex items)

order
```css
order: 5; /* default is 0 */
```

flex-grow
```css
flex-grow: 4; /* default 0 */
```

flex-shrink
```css
flex-shrink: 3; /* default 1 */
```

flex-basis
```css
flex-basis:  | auto; /* default auto */
```

flex: This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, like flex: 5;, that changes the flex-basis to 0%, so it’s like setting flex-grow: 5; flex-shrink: 1; flex-basis: 0%;.
```css
flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
```

align-self
```css
align-self: auto | flex-start | flex-end | center | baseline | stretch;
```


