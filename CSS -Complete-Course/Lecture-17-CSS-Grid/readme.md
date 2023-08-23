# Lecture - 17 CSS Grid

## Grid Layout

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

[![CSS Grid Container](https://css-tricks.com/wp-content/uploads/2018/11/align-content-stretch.svg)](https://www.youtube.com/@futureprogramming){:target="_blank"}

## Grid Elements

A grid layout consists of a parent element, with one or more child elements.

```html
<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>
</div>
```

## Display Property

An HTML element becomes a grid container when its display property is set to grid or inline-grid.

```css
.grid-container {
  display: grid;
}
```

All direct children of the grid container automatically become grid items.

## Grid Columns

The vertical lines of grid items are called columns.

![Gird Colmuns](https://www.w3schools.com/css/grid_columns.png)

### Grid Rows

The horizontal lines of grid items are called rows.

![Grid Rows](https://www.w3schools.com/css/grid_rows.png)

~~~~#### Grid Lines

The lines between columns are called column lines.

The lines between rows are called row lines.

![Grid Lines](https://www.w3schools.com/css/grid_lines.png)

Place a grid item at column line 1, and let it end on column line 3:

```css
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
```

## Grid Container Properties

Here are some of the CSS Grid Container properties:
`display`
`grid-template-columns`
`grid-template-rows`
`grid-template-areas`
`grid-template`
`grid-column-gap`
`grid-row-gap`
`grid-gap`
`justify-items`
`align-items`
`place-items`
`justify-content`
`align-content`
`place-content`
`grid-auto-columns`
`grid-auto-rows`
`grid-auto-flow`

### `grid-template-columns`

The grid-template-columns property defines the number of columns in your grid layout, and it can define the width of each column.

The value is a space-separated-list, where each value defines the width of the respective column.

If you want your grid layout to contain 4 columns, specify the width of the 4 columns, or "auto" if all columns should have the same width.

Make a grid with 4 columns:

```css
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto;
}
```

Note: If you have more than 4 items in a 4 columns grid, the grid will automatically add a new row to put the items in.

The grid-template-columns property can also be used to specify the size (width) of the columns.

```css
Example
Set a size for the 4 columns:

.grid-container {
  display: grid;
  grid-template-columns: 80px 200px auto 40px;
}
```

### `grid-template-rows`

The grid-template-rows property defines the height of each row. value is a space-separated-list, where each value defines the height of the respective row:

```css
Example
.grid-container {
  display: grid;
  grid-template-rows: 80px 200px;
}
```

### `justify-content`

The justify-content property is used to align the whole grid inside the container.

Note: The grid's total width has to be less than the container's width for the justify-content property to have any effect.

```css
Example
.grid-container {
  display: grid;
  justify-content: space-evenly;
}

.grid-container {
  display: grid;
  justify-content: space-around;
}

.grid-container {
  display: grid;
  justify-content: space-between;
}

.grid-container {
  display: grid;
  justify-content: center;
}
.grid-container {
  display: grid;
  justify-content: start;
}

.grid-container {
  display: grid;
  justify-content: end;
}
```

### `align-content`

The align-content property is used to vertically align the whole grid inside the container.

Note: The grid's total height has to be less than the container's height for the align-content property to have any effect.

```css
.grid-container {
  display: grid;
  height: 400px;
  align-content: center;
}

.grid-container {
  display: grid;
  height: 400px;
  align-content: space-evenly;
}

.grid-container {
  display: grid;
  height: 400px;
  align-content: space-around;
}


.grid-container {
  display: grid;
  height: 400px;
  align-content: space-between;
}

.grid-container {
  display: grid;
  height: 400px;
  align-content: start;
}

.grid-container {
  display: grid;
  height: 400px;
  align-content: end;
}
```

### `Grid Template Areas`

grid-template-areas CSS property specifies named grid areas, establishing the cells in the grid and assigning them names.

```css
grid-template-areas: "a b";
grid-template-areas:
  "a b b"
  "a c d";
```

### `Grid Template`

grid-template CSS property is a shorthand property for defining grid columns, grid rows, and grid areas.

```css
/* grid-template-rows / grid-template-columns values */
grid-template: 100px 1fr / 50px 1fr;
grid-template: auto 1fr / auto 1fr auto;
grid-template: [linename] 100px / [columnname1] 30% [columnname2] 70%;
grid-template: fit-content(100px) / fit-content(40%);

/* grid-template-areas grid-template-rows / grid-template-column values */
grid-template:
  "a a a"
  "b b b";
grid-template:
  "a a a" 20%
  "b b b" auto;
grid-template:
  [header-top] "a a a" [header-bottom]
  [main-top] "b b b" 1fr [main-bottom]
  / auto 1fr auto;
```

### Grid Gap

The spaces between each column/row are called gaps.

![Grid Gaps](https://www.w3schools.com/css/grid_gaps.png)

### `column-gap` property sets the gap between the columns

```css
.grid-container {
  display: grid;
  column-gap: 50px;
}
```

### `row-gap` property sets the gap between the rows

```css
.grid-container {
  display: grid;
  row-gap: 50px;
}
```

### `gap` property is a shorthand property for the row-gap and the column-gap properties

```css
.grid-container {
  display: grid;
  gap: 50px 100px;
}
```

gap property can also be used to set both the row gap and the column gap in one value:

```css
.grid-container {
  display: grid;
  gap: 50px;
}
```

### `Justify Items`

justify-items property is set on the grid container to give child elements (grid items) alignment in the inline direction.

For pages in English, inline direction is left to right and block direction is downward.

For this property to have any alignment effect, the grid items need available space around themselves in the inline direction.

Tip: To align grid items in block direction instead of inline direction, use align-items property.

```css
#container {
  display: grid;
  justify-items: end;
}
```

### Aling Items

In Grid Layout, it controls the alignment of items on the Block Axis within their grid area.

```css
#container {
  display: grid;
  position: relative;
  align-items: end;
}
```

### `place-items`

place-items shorthand property allows you to align items along both the block and inline directions at once (i.e. the align-items and justify-items properties) in a relevant layout system such as Grid or Flexbox. If the second value is not set, the first value is also used for it.

If the place-items property has two values:

place-items: start center;
align-items property value is 'start'
justify-items property value is 'center'
If the place-items property has one value:

place-items: end;
align-items and justify-items property values are both 'end'

```css
#container {
  place-items: start center;
}
```

### Place content

place-content property is used in flexbox and grid layouts, and is a shorthand property for the following properties:

align-content
justify-content
If the place-content property has two values:

place-content: start center;
align-content property value is 'start'
justify-content property value is 'center'
If the place-content property has one value:

place-content: end;
align-content and justify-content property values are both 'end'

```css
#container
{place-content: end space-between;
place-content: space-around start;
place-content: start space-evenly;
place-content: end center;
place-content: end;
}
```

### grid-auto-columns

grid-auto-columns CSS property specifies the size of an implicitly-created grid column track or pattern of tracks.

```css
grid-auto-columns: auto;
grid-auto-columns: 1fr;
grid-auto-columns: min-content;
grid-auto-columns: minmax(10px, auto);

## CSS Grid Items Properties
```

### `grid-auto-rows`

grid-auto-rows CSS property specifies the size of an implicitly-created grid row track or pattern of tracks.

```css
grid-auto-rows: min-content;
grid-auto-rows: max-content;
grid-auto-rows: auto;
grid-auto-rows: 100px;

```

### `grid-auto-flow`

grid-auto-flow property controls how auto-placed items get inserted in the grid. how the auto-placement algorithm works, specifying exactly how auto-placed items get flowed into the grid.

```css
grid-auto-flow: row;
grid-auto-flow: column;
grid-auto-flow: dense;
grid-auto-flow: row dense;
grid-auto-flow: column dense;
```

## Grid Items Properties

Child Elements (Items)
A grid container contains grid items.

By default, a container has one grid item for each column, in each row, but you can style the grid items so that they will span multiple columns and/or rows.

### grid-column

grid-column property defines on which column(s) to place an item.

You define where the item will start, and where the item will end.

Note: The grid-column property is a shorthand property for the grid-column-start and the grid-column-end properties.

To place an item, you can refer to line numbers, or use the keyword "span" to define how many columns the item will span.

```css
Example
Make "item1" start on column 1 and end before column 5:

.item1 {
  grid-column: 1 / 5;
}

Example
Make "item1" start on column 1 and span 3 columns:

.item1 {
  grid-column: 1 / span 3;
}

Example
Make "item2" start on column 2 and span 3 columns:

.item2 {
  grid-column: 2 / span 3;
}
```

grid-row Property:
The grid-row property defines on which row to place an item.

You define where the item will start, and where the item will end.

Note: The grid-row property is a shorthand property for the grid-row-start and the grid-row-end properties.

To place an item, you can refer to line numbers, or use the keyword "span" to define how many rows the item will span:

```css
Example
Make "item1" start on row-line 1 and end on row-line 4:

.item1 {
  grid-row: 1 / 4;
}

Example
Make "item1" start on row 1 and span 2 rows:

.item1 {
  grid-row: 1 / span 2;
}
```

grid-area Property
The grid-area property can be used as a shorthand property for the grid-row-start, grid-column-start, grid-row-end and the grid-column-end properties.


```css
Example
Make "item8" start on row-line 1 and column-line 2, and end on row-line 5 and column line 6:


.item8 {
  grid-area: 1 / 2 / 5 / 6;
}

Example
Make "item8" start on row-line 2 and column-line 1, and span 2 rows and 3 columns:

.item8 {
  grid-area: 2 / 1 / span 2 / span 3;
}

```

Naming Grid Items
The grid-area property can also be used to assign names to grid items.

Named grid items can be referred to by the grid-template-areas property of the grid container.

```css
Example
Item1 gets the name "myArea" and spans all five columns in a five columns grid layout:

.item1 {
  grid-area: myArea;
}
.grid-container {
  grid-template-areas: 'myArea myArea myArea myArea myArea';
}
```

Each row is defined by apostrophes (' ')

The columns in each row is defined inside the apostrophes, separated by a space.

Note: A period sign represents a grid item with no name.

Example
Let "myArea" span two columns in a five columns grid layout (period signs represent items with no name):

```css
.item1 {
  grid-area: myArea;
}
.grid-container {
  grid-template-areas: 'myArea myArea . . .';
}
```

To define two rows, define the column of the second row inside another set of apostrophes:

```css
Example
Make "item1" span two columns and two rows:

.grid-container {
  grid-template-areas: 'myArea myArea . . .' 'myArea myArea . . .';
}

Example
Name all items, and make a ready-to-use webpage template:

.item1 { grid-area: header; }
.item2 { grid-area: menu; }
.item3 { grid-area: main; }
.item4 { grid-area: right; }
.item5 { grid-area: footer; }

.grid-container {
  grid-template-areas:
    'header header header header header header'
    'menu main main main right right'
    'menu footer footer footer footer footer';
}
```

Order of the Items
The Grid Layout allows us to position the items anywhere we like.

The first item in the HTML code does not have to appear as the first item in the grid.

```css
Example
.item1 { grid-area: 1 / 3 / 2 / 4; }
.item2 { grid-area: 2 / 3 / 3 / 4; }
.item3 { grid-area: 1 / 1 / 2 / 2; }
.item4 { grid-area: 1 / 2 / 2 / 3; }
.item5 { grid-area: 2 / 1 / 3 / 2; }
.item6 { grid-area: 2 / 2 / 3 / 3; }
```

You can re-arrange the order for certain screen sizes, by using media queries:

```css
Example
@media only screen and (max-width: 500px) {
  .item1 { grid-area: 1 / span 3 / 2 / 4; }
  .item2 { grid-area: 3 / 3 / 4 / 4; }
  .item3 { grid-area: 2 / 1 / 3 / 2; }
  .item4 { grid-area: 2 / 2 / span 2 / 3; }
  .item5 { grid-area: 3 / 1 / 4 / 2; }
  .item6 { grid-area: 2 / 3 / 3 / 4; }
}
```