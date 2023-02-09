# Learn Flexbox

The Flexible Box Model is a one dimensional layout model that provides a
method to offer space distribution and powerful alignment capabilities.

- Before Flexbox, we aligned elements using floats and tables. Flexbox has
  made life much easier for people that use Css.
- CSS Grid is another option for alignment, positioning, etc. It's good to learn
  both.

## Flex Containers & Flex Items

The flex container is the element that holds flex items. Flex items are direct
children of flex containers. A container is created with display: flex

```
<div class="flex-container"> //container
    <div>Flex Item 1</div> //flex-items
    <div>Flex Item 2</div> //flex-items
    <img src="pic.png" alt="alternative-text-to-image" /> //flex-items
</div>
```

### Flex container and Flex Items has specific CSS property alloted to them.

![image](https://user-images.githubusercontent.com/52499108/217751356-272d9f96-8cda-402e-86ce-4d484cd0a7de.png)

### Flex Axes

When the flex container has a flex-direction of row, the main axis runs horizontally from left to right and the cross axis runs vertically from top to bottom. When the flex-direction is set to column, the main axis runs vertically from top to bottom and the cross axis runs horizontally from left to right.

![image](https://user-images.githubusercontent.com/52499108/217752846-ae5627f9-35f2-4aca-a539-00ed34051b3d.png)

### Properties

1. When container is set to `display:flex`.

```html
<body>
  <div class="flex-container">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
  </div>
</body>
```

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}

.flex-container {
  display: flex;
}

.item {
  width: 100px;
  height: 100px;
  background-color: chartreuse;
  border: 1px solid black;
  margin: 5px;
}
```

![image](https://user-images.githubusercontent.com/52499108/217771393-4105d286-14c4-4889-a326-399a3ba2accf.png)

2. When flex-direction is set to column.

```html
<body>
  <div class="flex-container">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
  </div>
</body>
```

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}

.flex-container {
  display: flex;
  flex-direction: column;
}

.item {
  width: 100px;
  height: 100px;
  background-color: chartreuse;
  border: 1px solid black;
  margin: 5px;
}
```

![image](https://user-images.githubusercontent.com/52499108/217787042-be6b22c9-ecec-44ca-8b52-8a2d41c3015d.png)

3. property: `justify-content`

"Justify content" in flexbox refers to the horizontal alignment of items within a flex container. It determines how the items are spread out along the main axis of the container.

There are several options for justifying content in flexbox, including:

- "Flex-start": This aligns all items to the start of the container.
- "Flex-end": This aligns all items to the end of the container.
- "Center": This aligns all items in the center of the container.
- "Space-between": This spreads out the items evenly across the container, with equal space between each item.
- "Space-around": This spreads out the items evenly across the container, with equal space around each item.

By choosing a justify content value, you can control how elements are laid out in a flexible container and create a clean, professional design for your website or application.

**Justify content for flex-direction: row**
![image](https://user-images.githubusercontent.com/52499108/217788941-691bbf00-82af-4058-8fbe-f3a05265fceb.png)

**Justify content for flex-direction: column**
**You have to have height to use this**

![image](https://user-images.githubusercontent.com/52499108/217789339-c4ccc564-8f54-47fe-9a73-1921d9ee847f.png)

4. Align items in flexbox refers to the vertical alignment of items within a flex container. It determines how the items are aligned along the cross axis of the container.

Just like with justify content, there are several options for aligning items in flexbox, including:

- "Flex-start": This aligns all items to the start of the container.
- "Flex-end": This aligns all items to the end of the container.
- "Center": This aligns all items in the center of the container.
- "Baseline": This aligns all items along their baselines.
- "Stretch": This stretches all items to fill the full height of the container.

By choosing an align items value, you can control the vertical positioning of elements within a flexible container and create a visually appealing design for your website or application.
