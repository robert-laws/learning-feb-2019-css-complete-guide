# Learning - Udemy: CSS - The Complete Guide (incl. Flexbox, Grid & Sass)

[Website for Course](https://learning-feb-2019-css-complete-guide.netlify.com)

[![Netlify Status](https://api.netlify.com/api/v1/badges/3996aefd-c1bc-484d-8417-fd25da0e1d89/deploy-status)](https://app.netlify.com/sites/learning-feb-2019-css-complete-guide/deploys)

**Table of Contents**

* [CSS Basics](#css-basics)
* [Beyond the Basics](#beyond-the-basics)

## CSS Basics

Getting started with CSS syntax. What is the rationale for using CSS?

CSS = Cascading Styles Sheets

* HTML is used for structure of page
* CSS is used for styling of the website

```css
/* Basic Syntax - selector and properties with values */
div {
  color: #F00;
  font-size: 1.5rem;
}
```

### CSS Combinators

**Adjacent Sibling**

The second element shares the same parent as the first element and comes immediately after the first.

```html
<div>
  <h1>Welcome</h1>
  <h2>Greetings from your support team</h2>
</div>
```

```css
h1 + h2 {
  color: red;
}
```

**General Sibling**

The second element has the same parent and comes at any location - immediately after or after other elements.

```html
<div>
  <h1>Welcome</h1>
  <p>There is a lot of information available here</p>
  <ul>
    <li>Program dates</li>
    <li>Activities</li>
  </ul>
</div>
```

```css
h1 ~ ul {
  font-size: 2rem;
}
```

**Child Combinator**

The second element is the direct child of the first element.

```html
<p>Some good <span>information</span> is found here</p>
```

```css
p > span {
  color: red
}
```

**General Descendant**

The second element is the child of the first element.

```html
<ul>
  <li>Name</li>
  <li>Activities
    <ul>
      <li>Boating</li>
      <li>Swimming <span>* with approval</span></li>
      <li>Hiking</li>
    </ul>
  </li>
  <li>Locations</li>
</ul>
```

```css
ul span {
  color: blue;
}
```

## Beyond the Basics