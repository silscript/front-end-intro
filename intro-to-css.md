# Front-End Development Part #2
The practice of producing HTML, CSS, and JavaScript for a website or web application for a user to interact with it directly.

## Cascading Style Sheets
CSS stands for cascading style sheets. CSS is used to define style for your webpages, such as the design and layout for different devices and screen sizes. With an external stylesheet file, it's easy changing the styles for an entire website.

- Let's style our website! Add your own styles and have fun!
- Create a styles.css file within the same directory as your index.html file.
- As we go, add different css rules we will be using throughout the class.
- CSS rules consists of a selector (attribute, class, id, tagname, etc.) and a declaration block (a property and a value).
- Declaration blocks end with a semicolon and are surrounded by curly braces.
- `selector` is the element you want to style.
- `property` is the name of the property.
- `value` is the value of the property.

```css
selector {
  property: value;
}
```

```css
div {
  background-color: #000000;
}
```

###### Element Selectors:
- The element selector selects elements based on the element name.
- For example, `<html>, <body>, <header>, <main>, <div>, <h1>, <p>,` etc.

```html
<div>
  <!-- Content -->
</div>
```

```css
div {
  background-color: #000000;
}
```

###### Class Selectors:
- The class selector selects elements with a specific class attribute.
- To select elements with a specific class, add a `.` before the name of the class.
- Never start a class name with a number!

```html
<div class="site-container">
  <!-- Content -->
</div>
```

```css
.site-container {
  background-color: #000000;
}
```

- You can also specify that only specific HTML elements should be affected by a class.
- All `<div>` elemets with a `class="site-container"` will be changed.

```css
div.site-container {
  background-color: #000000;
}
```

###### ID Selectors:
- The id selector uses the id attribute of an HTML element to select a specific element.
- An id should be unique within a page, so the id selector is used if you want to select a single, unique element.
- To select elements with a specific id, add a `#` before the name of the id.

```html
<div id="site-container">
  <!-- Content -->
</div>
```

```css
#site-container {
  background-color: #000000;
}
```

###### Grouping Selectors:
- If you have elements with the same style definitions, group them!
- You can group the selectors, to minimize the code.

```css
header {
  background-color: #000000;
}

footer {
  background-color: #000000;
}

div {
  background-color: #000000;
}
```

- Minimizing your code is important. Faster upload time, easier to read, consistent edits.
- To group selectors, separate each selector with a comma. So cool!

```css
header, footer, div {
  background-color: #000000;
}
```

###### Specificity:
- Specificity determines which CSS rule is applied by the browsers.
- If two selectors apply to the same element, the one with higher specificity wins.
- The last rule defined overrides any previous, conflicting rules.
- There are four distinct categories which define the specificity level of a given selector:
  - Inline styles.
  - ID selectors.
  - Class and attribute selectors.
  - Element selectors.
- It's important to structure your CSS file to avoid unexpected overrides.

###### Box Model:
- The box model describes how all block elements behave.
- It wraps around every HTML element. It consists of:
  - Margins - Clears an area outside the border. The margin is transparent.
  - Borders - The border goes around the padding and content
  - Padding - Clears an area around the content. The padding is transparent.
  - Content - The content (images and text) of the box.
- In order to set the width and height of an element correctly in all browsers, you need to calculate the size of the content, padding, borders and margins.
- However, we can avoid calculating by altering the default CSS box model.
- `box-sizing: border-box;` includes the padding and border to the width and height, but not the margin.

```css
html {
  box-sizing: border-box;
}

*, *::before, *::after {
  box-sizing: inherit;
}
```

###### Colors:
- Colors are displayed by combining red, green, and blue light.
- Colors are defined using a hexadecimal (HEX) notation (#000000) for the combination of RGB values.
- The lowest hexadecimal value is 0 (HEX 00). This darkens the color value.
- The highest value is 255 (HEX FF). This brightens the color value.

```css
div {
  background-color: #000000 /* Black */
}

div {
  background-color: #FFFFFF /* White */
}

div {
  background-color: #FF0000 /* Red */
}

div {
  background-color: #00FF00 /* Green */
}

div {
  background-color: #0000FF /* Blue */
}
```

###### Typography Units:
- The main units in CSS are `em`, `px`, `pt`, `%`.
- The `em` is a scalable unit that is used in a document.
- It is equal to the current font-size, for instance, if the font-size of the document is 12pt, 1em is equal to 12pt.

```css
body {
  font-size: 62.5%; /* 1em = 10px */
}

h1 {
  font-size: 1em;
}
```

- Pixels are fixed-size units that are used in screen media (i.e. to be read on the computer screen).
- One pixel is equal to one dot on the computer screen (the smallest division of your screen’s resolution).

```css
h1 {
  font-size: 12px;
}
```

- Points are traditionally used in print media (anything that is to be printed on paper, etc.).
- One point is equal to 1/72 of an inch.
- Points are much like pixels, in that they are fixed-size units and cannot scale in size.

```css
h1 {
  font-size: 12pt;
}
```

- The percent unit is much like the “em” unit, save for a few fundamental differences.
- The current font-size is equal to 100% (i.e. 12pt = 100%).
- While using the percent unit, your text remains fully scalable for mobile devices and for accessibility.

```css
h1 {
  font-size: 100%;
}
```

Use ems! Please!

###### :
- If a font name contains white-space, it must be quoted.

## That's All! (4:10pm)
![Mind Blown!](https://raw.githubusercontent.com/silscript/front-end-intro/master/assets/pug_amazed.gif)

## Credits
- Animated pug gifs from Space Brothers.
- Various content by W3Schools.

## Resources
A list of CSS resources that I frequently use:
- Can I Use: http://caniuse.com/
- CodePen: http://codepen.io/
- CSS-Tricks: https://css-tricks.com/
- CSS Colors: http://www.colors.commutercreative.com/
- CSS Colours: http://colours.neilorangepeel.com/
- CSS Specificity: http://specificity.keegan.st/
- Font Awesome Icons: https://fortawesome.github.io/Font-Awesome/icons/
- Google Fonts: https://www.google.com/fonts
- Mozilla Docs: https://developer.mozilla.org/en-US/
- Stack Overflow: http://stackoverflow.com/

## Contact Information
If you have any questions, don't hesitate to contact me! :)
- Email: silscript@gmail.com
- Dribbble: https://dribbble.com/silscript
- GitHub: https://github.com/silscript
- Twitter: http://twitter.com/silscript
