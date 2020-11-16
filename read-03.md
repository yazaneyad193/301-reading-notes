# Read 03

## JavaScript Templating

Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic. The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

### Mustache

Mustache.js is a zero-dependency implementation of the mustache template system in JavaScript.
Mustache is a logic-less template syntax. It can be used for HTML, config files, source code - anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.

Example on mustache.js:

```javascript

Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn

```

## Flex

CSS Flexible Box Layout is a module of CSS that defines a CSS box model optimized for user interface design, and the layout of items in one dimension. In the flex layout model, the children of a flex container can be laid out in any direction, and can “flex” their sizes, either growing to fill unused space or shrinking to avoid overflowing the parent. Both horizontal and vertical alignment of the children can be easily manipulated.

The Flexible Box Module, usually referred to as flexbox, was designed as a one-dimensional layout model, and as a method that could offer space distribution between items in an interface and powerful alignment capabilities. This article gives an outline of the main features of flexbox, which we will be exploring in more detail in the rest of these guides.

When we describe flexbox as being one dimensional we are describing the fact that flexbox deals with layout in one dimension at a time — either as a row or as a column. This can be contrasted with the two-dimensional model of CSS Grid Layout, which controls columns and rows together.

### Properties for the Parent (flex container)

| Property | Usage | Values |
|----|----|----|
| display | This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children. | `flex` |
| flex-direction | This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns. | `row`, `row-reverse`, `column`, `column-reverse` |
| flex-wrap | By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property. | `nowrap`, `wrap`, `wrap-reverse` |
| justify-content | This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line. | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly` |
| flex-flow | This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap. | `column wrap` |
| align-items | This defines the default behavior for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis (perpendicular to the main-axis). | `stretch`, `flex-start`, `flex-end`, `center`, `baseline` |
| align-content | This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis. | `normal`, `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`, `stretch`|

### Properties for the Children (flex items)

| Property | Usage | Values |
|----|----|----|
| order | By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container. | `0`, `1`, `2` |
| flex-grow | This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up. If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children. If one of the children has a value of 2, the remaining space would take up twice as much space as the others (or it will try to, at least). | `0`, `1`, `2` |
| flex-shrink | This defines the ability for a flex item to shrink if necessary. | `1`, `2`, `3` |
| flex-basis | This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.) or a keyword. The auto keyword means “look at my width or height property” (which was temporarily done by the main-size keyword until deprecated). The content keyword means “size it based on the item’s content” – this keyword isn’t well supported yet, so it’s hard to test and harder to know what its brethren max-content, min-content, and fit-content do. | `0`, `auto` |
| flex | This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0. | `none` |
| align-self | This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items. Please see the align-items explanation to understand the available values. | `stretch`, `flex-start`, `flex-end`, `center`, `baseline` |

[Back to Home](README.md)
