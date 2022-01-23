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

Additional resources:
[CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
[justify-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items#Values)
[justify-content](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content#Values)
[align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items#Values)
[align-content](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content#values)
