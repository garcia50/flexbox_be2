
### Let's play

- Check out the `index.html` and `custom.css`
- Right now, we have two sections, each with 6 boxes (each 100px in width).
- We have not set the width on the `.boxes` sections so they are taking up the entire width of the page.

#### Display: flex;

- First things first, we want all of those boxes in the `section class="boxes-1` to be in a row, not a column but because of the default properties of a `div` being block, each one of these boxes is stacked on top of each other.

```css
.boxes-1 {
  display: flex;
}
```

- Each child of a flex container becomes a flex item. Text directly contained in a flex container is wrapped in an anonymous flex item.

- This tells our `boxes-1` to turn into a flex container that we can now play with
- By default, this property aligns elements inline within that container

- What happened?
- Our boxes are set to their width of 100px and now in a row.
- We can also adjust the width and height of the section that is containing the boxes and the boxes themselves.

#### Flex-wrap

- Let's change the size of our boxes to 500px and see what happens
- No matter how big the original boxes were, they will all fit into that section unless we change that option!

```css
.boxes {
  display: flex;
  flex-wrap: wrap;
}
```

#### Justify-Content

- We can play with where the contents sits within this section!
- We want to center the boxes in this section.

```css
.boxes-1 {
  display: flex;
  justify-content: center;
}
```

- Other options: `space-around`, `space-between`, `flex-start`(default), `flex-end`

#### Flex-direction

- By default, the direction is `row` but we can use other options such as `column` and both in reverse, `column-reverse` and `row-reverse`
- Let's reverse our row in `boxes-1`

  ```css
    .boxes-1 {
      flex-direction: row-reverse;
    }
  ```

- A shorthand for both `flex-wrap` and `flex-direction` is `flex-flow`

#### All Boxes Flex

- What about the other section of boxes?
- Let's flex `.all-boxes` and apply the some flexbox rules to it.

```css
.all-boxes {
  display: flex;
}
```
