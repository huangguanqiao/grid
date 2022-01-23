## Justify Items
justify-items is a property that positions grid items along the inline, or row, axis. This means that it positions items from left to right across the web page. This property is declared on grid containers. 
justify-items属性设置单元格内容的水平位置（左中右）

`justify-items: start | end | center | stretch;`

justify-items accepts these values:
- start — aligns grid items to the left side of the grid area 对齐单元格的起始边缘。
- end — aligns grid items to the right side of the grid area 对齐单元格的结束边缘。
- center — aligns grid items to the center of the grid area 单元格内部居中。
- stretch — stretches all items to fill the grid area 拉伸，占满单元格的整个宽度（默认值）

## Justify Content
We can use justify-content to position the entire grid along the row axis. This property is declared on grid containers.
justify-content属性是整个内容区域在容器里面的水平位置（左中右）

`justify-content: start | end | center | stretch | space-around | space-between | space-evenly;`

It accepts these values:
- start — aligns the grid to the left side of the grid container
- end — aligns the grid to the right side of the grid container
- center — centers the grid horizontally in the grid container
- stretch — stretches the grid items to increase the size of the grid to expand horizontally across the container
- space-around — includes an equal amount of space on each side of a grid element, resulting in double the amount of space between elements as there is before the first and after the last element
- space-between — includes an equal amount of space between grid items and no space at either end
- space-evenly — places an even amount of space between grid items and at either end

## Align Items
align-items is a property that positions grid items along the block, or column axis. This means that it positions items from top to bottom. This property is declared on grid containers. 
align-items属性设置单元格内容的垂直位置（上中下）

`align-items: start | end | center | stretch;`

align-items accepts these values:
- start — aligns grid items to the top side of the grid area 对齐单元格的起始边缘。
- end — aligns grid items to the bottom side of the grid area 对齐单元格的结束边缘。
- center — aligns grid items to the center of the grid area 单元格内部居中。
- stretch — stretches all items to fill the grid area 拉伸，占满单元格的整个宽度（默认值）

## Align Content
align-content positions the rows along the column axis, or from top to bottom, and is declared on grid containers.
align-content属性是整个内容区域的垂直位置（上中下）

`align-content: start | end | center | stretch | space-around | space-between | space-evenly;`

It accepts these positional values:

- start — aligns the grid to the top of the grid container
- end — aligns the grid to the bottom of the grid container
- center — centers the grid vertically in the grid container
- stretch — stretches the grid items to increase the size of the grid to expand vertically across the container
- space-around — includes an equal amount of space on each side of a grid element, resulting in double the amount of space between elements as there is before the first and after the last element
- space-between — includes an equal amount of space between grid items and no space at either end
- space-evenly — places an even amount of space between grid items and at either end

## Justify Self and Align Self
justify-self specifies how an individual element should position itself with respect to the row axis. This property will override justify-items for any item on which it is declared.

align-self specifies how an individual element should position itself with respect to the column axis. This property will override align-items for any item on which it is declared.

1. justify-self属性设置单元格内容的水平位置（左中右），跟justify-items属性的用法完全一致，但只作用于单个项目。
2. align-self属性设置单元格内容的垂直位置（上中下）， 跟align-items属性的用法完全一致，也是只作用于单个项目。
3. place-self属性是align-self属性和justify-self属性的合并简写形式。

```CSS
justify-self: start | end | center | stretch;
align-self: start | end | center | stretch;
place-self: <align-self> <justify-self>;

//start：对齐单元格的起始边缘。
//end：对齐单元格的结束边缘。
//center：单元格内部居中。
//stretch：拉伸，占满单元格的整个宽度（默认值）。
```
- start — positions grid items on the left side/top of the grid area
- end — positions grid items on the right side/bottom of the grid area
- center — positions grid items on the center of the grid area
- stretch — positions grid items to fill the grid area (default)

## Grid Auto Rows and Grid Auto Columns
grid-auto-rows specifies the height of implicitly added grid rows. grid-auto-columns specifies the width of implicitly added grid columns.
用来设置，浏览器自动创建的多余网格的列宽和行高。

grid-auto-rows and grid-auto-columns accept the same values as their explicit counterparts, grid-template-rows and grid-template-columns:

- pixels (px)
- percentages (%)
- fractions (fr)
- the repeat() function

## Grid Auto Flow
grid-auto-flow specifies whether new elements should be added to rows or columns, and is declared on grid containers.

grid-auto-flow accepts these values:
划分网格以后，容器的子元素会按照顺序，自动放置在每一个网格。默认的放置顺序是"先行后列"，即先填满第一行，再开始放入第二行，即下图数字的顺序。

```CSS
// 这个顺序由grid-auto-flow属性决定，默认值是row，即"先行后列"。也可以将它设成column，变成"先列后行"。
grid-auto-flow: column;

```

- row — specifies the new elements should fill rows from left to right and create new rows when there are too many elements (default)
- column — specifies the new elements should fill columns from top to bottom and create new columns when there are too many elements
- dense — this keyword invokes an algorithm that attempts to fill holes earlier in the grid layout if smaller elements are added
You can pair row or column with dense, like this: grid-auto-flow: row dense;.

## Review
Great work! You have learned many new properties to use when creating a layout using CSS Grid! Let’s review:

- grid-template-areas specifies grid named grid areas
- grid layouts are two-dimensional: they have a row, or inline, axis and a column, or block, axis.
- justify-items specifies how individual elements should spread across the row axis
- justify-content specifies how groups of elements should spread across the row axis
- justify-self specifies how a single element should position itself with respect to the row axis
- align-items specifies how individual elements should spread across the column axis
- align-content specifies how groups of elements should spread across the column axis
- align-self specifies how a single element should position itself with respect to the column axis
- grid-auto-rows specifies the height of rows added implicitly to the grid
- grid-auto-columns specifies the width of columns added implicitly to the grid
- grid-auto-flow specifies in which direction implicit elements should be created

Additional resources:
[CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
[justify-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items#Values)
[justify-content](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content#Values)
[align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items#Values)
[align-content](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content#values)
