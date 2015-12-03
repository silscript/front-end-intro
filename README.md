# Front-End Development
The practice of producing HTML, CSS, and JavaScript for a website or web application for a user to interact with it directly.

## Learning Objectives (5min)
- Differentiate between HTML and CSS.
- Explain how HTML is used for content.
- Explain how CSS is used for styling.
- Inspect an element using development tools.
- Know which content goes in the head.
- Know which content goes in the body.
- Link a stylesheet to HTML.
- Utilize common css properties.

## Introduce Yourself! (10min)
Let's get to know each other!
- What is your name?
- Where are you from?
- What do you do?
- Which superhero would you be and why?

## Opening Framing! (5min)
- What brings you all here today?
- What would you all like to accomplish?

## Set Up Chatroom! (2min)
In order to share links, please use this site to chat.
- https://chatstep.com/
- Add your name and the password.
- It's secure and private!

## Website Preparation (10min)
In order to build and deploy a website or web application, you will need certain requirements. Today, we will be using Google Chrome as our browser and Sublime Text as our editor. If you are unable to install Sublime Text due to having a work computer or anything else, let us know! You may need to use the default text editor.

###### Requirements:
- A computer (Acer, Dell, Lenova, MacBook, Surface Pro, etc.).
- A web browser ([Chrome](https://www.google.com/chrome/browser/desktop/), [Edge](https://www.microsoft.com/en-us/download/details.aspx?id=48126), [FireFox](https://www.mozilla.org/en-US/firefox/new/), [Internet Explorer](http://windows.microsoft.com/en-us/internet-explorer/download-ie), [Safari](https://support.apple.com/downloads/safari), and [Opera](http://www.opera.com/)).
- A text editor ([Atom](https://atom.io/), Notepad, [Sublime Text](http://www.sublimetext.com/3), and TextEdit).

###### Deployment:
- A FTP client ([Cyberduck](https://cyberduck.io/), [FileZilla](https://filezilla-project.org/), [SmartFTP](https://www.smartftp.com/), and [Transmit](https://panic.com/transmit/)).
- A domain name (assigning addresses to internet web servers).
- A host (serves the pages for one or more websites).
- We will be using [BitBalloon](https://www.bitballoon.com/)! It's free!

## Hyper Text Markup Language
HTML is a markup language for describing webpages. For example, let's visit the Google website! We will be using the developer tools to inspect the webpage. At the end of the day, a website is just content!

- Display elements in the developer tools.
- Let's create a rudimentary website! Add your own content and have fun!
- Create a new directory to contain your files and assets.
- Create an index.html file within that directory.
- As we go, add different elements we will be using throughout the class.
- Markup language is a set of markup tags.
- HTML tags describes different document content (important with SEO).
- HTML documents are described by HTML tags.
- HTML tags usually come in pairs.
- The first tag is the start (opening) tag, the second tag is the end (closing) tag.
- The end (closing) tag is written with a slash before the tag name.

```html
<tagname>content</tagname>
```

- `<!DOCTYPE html>` describes an HTML document.
- `<html></html>` defines the document type.
- `<head></head>` is the information about the document.
- `<body></body>` contains visible content.

```html
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```

- `<meta></meta>` describes metadata (information).
- `<meta charset="utf-8">` defines the character set for the document.
- `<title></title>` is the title of the document (important with SEO).
- `<meta name="description" content="...">` is the description of the document (important with SEO).
- `<link rel="shortcut icon" href="" type="image/x-icon">` is the favorite icon.
- `<link rel="stylesheet" href="">` links the CSS styles to the HTML document.
- Attributes provide additional information about an element.
  - Attributes are always specified in the start tag.
  - Attributes come in name/value pairs like: name="value".
  - Examples: alt, href, id, rel, src, style, etc.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <meta name="description" content="">
    <link rel="shortcut icon" href="" type="image/x-icon">
    <link rel="stylesheet" href="">
  </head>
  <body>
    Hello World!
  </body>
</html>
```

Open in the Chrome browser. Congratulations, you developed your first site!

##  HTML Elements
HTML5 offers new semantic elements to define parts of a document. A semantic element describes its meaning to the browser and defines its content. All semantic elements are supported in all modern browsers. In order to add content to a document, elements have to nest. That is, every element has to be completely inside another element.

###### Semantic Elements:
- `<header></header>` specifies a header for a document or for introductory content.
- `<nav></nav>` defines a set of navigation links.
- `<main></main>` specifies the main content of a document.
- `<section></section>` defines a thematic grouping of content.
- `<footer></footer>` specifies a footer for a document or section.
- You can have multiple headers, navs, sections, and footers, but can only have one main element.
- There are more semantic elements, but these are the important ones.

```html
<body>
  <header>
    <nav>
    </nav>
  </header>

  <main>
    <section>
    </section>
  </main>

  <footer>
  </footer>
</body>
```

- `<h1> - <h6>` defines HTML headings.
  - Use headings for heading only, do not use for style purposes.
  - Search engines use your heading to index the structure and content of your web pages.
  - `<h1></h1>` defines the most important heading.
  - `<h6></h6>` defines the least important heading.
- `<p></p>` defines a paragraph.
- `<ul></ul>` defines an unordered bulleted list.
- `<li></li>` defines a list item.
- `<a href=""></a>` defines a hyperlink, which is used to link from one page to another.
  - `href=""`specifies the url of the page the link goes to.
- `<img src="" alt="">`defines an image in an HTML page.
  - `src=""`specifies the url of an image.
  - `alt=""`specifies an alternate text for an image.

```html
<body>
    <header>
      <h1></h1>
      <h2></h2>
      <p></p>

      <nav>
        <ul>
          <!-- Add links. -->
          <li><a href=""></a></li>
          <li><a href=""></a></li>
          <li><a href=""></a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section>
        <!-- Add images with a url. -->
        <h1></h1>
        <img src="" alt="">
        <img src="" alt="">
      </section>

      <section>
        <!-- Add images with a path. -->
        <h1></h1>
        <img src="" alt="">
        <img src="" alt="">
      </section>
    </main>

    <footer>
      <p></p>
    </footer>
  </body>
```

###### Non-Semantic Elements:
- Both the `<div>` and `<span>` tell nothing about its content.
- `<div></div>` defines a division or a section in a document.
  - Used to group block-elements to format with CSS.
- `<span></span>` is used to group inline-elements in a document.
  - Tag provides no visual change by itself.

```html
<body>
    <header>
      <h1></h1>
      <h2></h2>
      <p><span></span></p>

      <nav>
        <ul>
          <!-- Add links. -->
          <li><a href=""></a></li>
          <li><a href=""></a></li>
          <li><a href=""></a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section>
        <!-- Add images with a url. -->
        <h1></h1>
        <img src="" alt="">
        <img src="" alt="">
      </section>

      <section>
        <!-- Add images with a path. -->
        <h1></h1>
        <img src="" alt="">
        <img src="" alt="">
      </section>

      <div>
        <!-- Add an image with a path or url. -->
        <img src="" alt="">
      </div>
    </main>

    <footer>
      <p></p>
    </footer>
  </body>
```

## Lunch Time! (1:00pm – 2:00pm)
![Lunch Time!](https://raw.githubusercontent.com/silscript/front-end-intro/master/assets/pug_eating.gif)

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

###### Box Model
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

###### Hex Values

###### Font Values
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
