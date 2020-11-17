# Read 04

## Regular Expressions (RegEx)

Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).

This syntax can be used in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

1. Anchors — ^ and $
2. Quantifiers — * + ? and {}
3. OR operator — | or []
4. Character classes — \d \w \s and .
5. Grouping and capturing — ()
6. Bracket expressions — []
7. Boundaries — \b and \B
8. Look-ahead and Look-behind — (?=) and (?<=)
9. Look-ahead and Look-behind — (?=) and (?<=)

## Grid

CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that element’s children (which become Grid Items).

### Properties for the Parent (Grid Container)

1. `display`: Defines the element as a grid container and establishes a new grid formatting context for its contents.
2. `grid-template-columns` and `grid-template-rows`: Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.
3. `grid-template-areas`: Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. Repeating the name of a grid area causes the content to span those cells. A period signifies an empty cell. The syntax itself provides a visualization of the structure of the grid.
4. `grid-template`: A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.
5. `column-gap`, `row-gap`, `grid-column-gap`, `grid-row-gap`: Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.
6. `gap`, `grid-gap`: A shorthand for row-gap and column-gap.

### Properties for the Children (Grid Items)

1. `grid-column-start`, `grid-column-end`, `grid-row-start`, `grid-row-end`: Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.
2. `grid-column`, `grid-row`: Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end, respectively.
3. `grid-area`: Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Alternatively, this property can be used as an even shorter shorthand for grid-row-start + grid-column-start + grid-row-end + grid-column-end.
4. `justify-self`: Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis). This value applies to a grid item inside a single cell.
5. `align-self`: Aligns a grid item inside a cell along the block (column) axis (as opposed to justify-self which aligns along the inline (row) axis). This value applies to the content inside a single grid item.
6. `place-self`: place-self sets both the align-self and justify-self properties in a single declaration.

[Back to Home](README.md)
