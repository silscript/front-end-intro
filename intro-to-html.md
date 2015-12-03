# Front-End Development Part #1
The practice of producing HTML, CSS, and JavaScript for a website or web application for a user to interact with it directly.

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

## Credits
- Animated pug gifs from Space Brothers.
- Various content by W3Schools.

## Resources
A list of HTML resources that I frequently use:
- CodePen: http://codepen.io/
- GitHub: https://github.com/
- HTML5 Doctor: http://html5doctor.com/
- Mozilla Docs: https://developer.mozilla.org/en-US/
- Stack Overflow: http://stackoverflow.com/

## Contact Information
If you have any questions, don't hesitate to contact me! :)
- Email: silscript@gmail.com
- Dribbble: https://dribbble.com/silscript
- GitHub: https://github.com/silscript
- Twitter: http://twitter.com/silscript
