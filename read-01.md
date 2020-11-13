# Read 01

## Responsive Web Design

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

### Responsive vs. Adaptive vs. Mobile

Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference. Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing, all of which can become an obstacle for both developers and users.

The most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.

### Flexible Layouts

Responsive web design is broken down into three main components, including:

1. Flexible layouts
2. Media queries
3. Flexible media

|Relative Viewport Lengths CSS Properties | Meaning |
|----|----|
| `vw` | Viewports width |
| `vh` | Viewports height |
| `vmin` | Minimum of the viewport’s height and width |
| `vmax` | Maximum of the viewport’s height and width |

### Media Queries

Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.

There are a couple different ways to use media queries, using the `@media` rule inside of an existing style sheet, importing a new style sheet using the `@import` rule, or by linking to a separate style sheet from within the HTML document.

Example:

```css

/* @media Rule */
@media all and (max-width: 1024px) {...}

/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}

```

## Float

Float is a CSS positioning property. In web design, page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them.

| Float property values | What they do |
|----|----|
| `float: left` | floats element to left |
| `float: right` | floats element to right |
| `float: none` | enusres the element will not float (default) |
| `float: inherit` | assumes the float value from the parent element |

Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

## SMACSS

SMACSS (pronounced “smacks”) is more style guide than rigid framework. There is no library within here for you to download or install. There is no git repository for you to clone. SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.

[Back to Home](README.md)
