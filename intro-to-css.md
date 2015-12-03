# Front-End Development Part #2
The practice of producing HTML, CSS, and JavaScript for a website or web application for a user to interact with it directly.

## Cascading Style Sheets
CSS stands for cascading style sheets. CSS is used to define style for your webpages, such as the design and layout for different devices and screen sizes. With an external stylesheet file, it's easy changing the styles for an entire website.

- Let's style our website! Add your own styles and have fun!
- Create a styles.css file within the same directory as your index.html file.
- As we go, add different css rules we will be using throughout the class.
- CSS rules consists of a selector (attribute, class, id, tagname, etc.) and a declartion block (a property and a value).
- Declaration blocks end with a semicolon and are surrouned by curly braces.
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
- To group selectors, separate each selector with a comma.

```css
header, footer, div {
  background-color: #000000;
}
```

###### CSS Specificity
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

###### Hex Values:

###### Font Values:
- If a font name contains white-space, it must be quoted.


## Credits
- Animated pug gifs from Space Brothers.
- Font-Awesome Iconography by Dave Gandy.
- Name of Font by Name of Designer & Google Fonts.
- Various content by W3Schools.

## Resources
A list of resources that I use constantly:
- Can I Use: http://caniuse.com/
- CodePen: http://codepen.io/
- CSS-Tricks: https://css-tricks.com/
- CSS Colors: http://www.colors.commutercreative.com/
- CSS Colours: http://colours.neilorangepeel.com/
- CSS Specificity: http://specificity.keegan.st/
- Font Awesome Icons: https://fortawesome.github.io/Font-Awesome/icons/
- GitHub: https://github.com/
- Google Fonts: https://www.google.com/fonts
- HTML5 Doctor: http://html5doctor.com/
- Mozilla Docs: https://developer.mozilla.org/en-US/
- Stack Overflow: http://stackoverflow.com/

## Contact Information
If you have any questions, don't hesitate to contact me! :)
- Email: silscript@gmail.com
- Dribbble: https://dribbble.com/silscript
- GitHub: https://github.com/silscript
- Twitter: http://twitter.com/silscript
