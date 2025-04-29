This is the notes I have taken from [Responsive Web Design](https://www.freecodecamp.org/learn/2022/responsive-web-design) [https://www.freecodecamp.org/learn/](https://www.freecodecamp.org/learn/)

### 1

HTML elements have opening tags like `<h1>` and closing tags like `</h1>`. The text an element will display goes between its opening and closing tags.

### 2

The `h1` through `h6` heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so `h2` elements have less importance than `h1` elements.

Example Code

```html
<h1>most important heading element</h1>
<h2>second most important heading element</h2>
<h3>third most important heading element</h3>
<h4>fourth most important heading element</h4>
<h5>fifth most important heading element</h5>
<h6>least important heading element</h6>
```

Only use one `h1` element per page and place lower importance headings below higher importance headings.

### 3

The `p` element is used to create a paragraph of text on websites.

### 4

Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.

Here is an example of a comment with the `TODO: Remove h1`:

Example Code

```html
<!-- TODO: Remove h1 -->
```

### 5

HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

The `main` element is used to represent the main content of the body of an HTML document. Content inside the `main` element should be unique to the document and should not be repeated in other parts of the document.

Example Code

```html
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

Identify the main section of this page by adding a `<main>` opening tag before the `h1` element, and a `</main>` closing tag after the `p` element.

### 6

In the previous step, you put the `h1`, `h2`, comment, and `p` elements inside the `main` element. This is called *nesting*. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.

Here is an example of nesting and indentation:

Example Code

```html
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

The `h1` element, `h2` element and the comment are indented two spaces more than the `main` element in the code below.

### 7

You can add images to your website by using the `img` element. `img` elements have an opening tag without a closing tag. An element without a closing tag is known as a void element.

### 8

HTML attributes are special words used inside the opening tag of an element to control the element's behavior. The `src` attribute in an `img` element specifies the image's URL (where the image is located).

Here is an example of an `img` element with a `src` attribute pointing to the freeCodeCamp logo:

Example Code

```html
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg" />
```

### 9

All `img` elements should have an `alt` attribute. The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

Here is an example of an `img` element with an `alt` attribute:

Example Code

```html
<img src="cat.jpg" alt="A cat" />
```

### 10

You can link to another page with the anchor (`a`) element.

Here is an example linking to `https://www.freecodecamp.org`:

Example Code

```html
<a href="https://www.freecodecamp.org"></a>
```

### 11

A link's text must be placed between the opening and closing tags of an anchor (`a`) element.

Here is an example of a link with the text `click here to go to freeCodeCamp.org`:

Example Code

```html
<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>
```

### 12

In previous steps you used an anchor element to turn text into a link. Other types of content can also be turned into a link by wrapping it in anchor tags.

Here is an example of turning an image into a link:

Example Code

```html
<a href="example-link">
  <img src="image-link.jpg" alt="A photo of a cat." />
</a>
```

### 13

Before adding any new content, you should make use of a `section` element to separate the cat photos content from the future content.

The `section` element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.

Example Code

```html
<section>
  <h2>Section Title</h2>
  <p>Section content...</p>
</section>
```

Take your `h2`, `p`, and anchor (`a`) elements and nest them in a `section` element.

### 14

The `li` element is used to create a list item in an ordered or unordered list.

Here is an example of list items in an unordered list:

Example Code

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

### 15

The `figure` element represents self-contained content and will allow you to associate an image with a caption.

### 16

A figure caption (`figcaption`) element is used to add a caption to describe the image contained within the `figure` element.

Here is an example of a `figcaption` element with the caption of `A cute cat`:

Example Code

```html
<figure>
  <img src="image.jpg" alt="A description of the image" />
  <figcaption>A cute cat</figcaption>
</figure>
```

After the image nested in the `figure` element, add a `figcaption` element with text.

### 17

To place emphasis on a specific word or phrase, you can use the `em` element.

```html
<figcaption>Cats <em>love</em> lasagna.</figcaption>
```

![[em.png]]

### 18

The code for an ordered list (`ol`) is similar to an unordered list, but list items in an ordered list are numbered when displayed.

```html
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>
```

### 19

The `strong` element is used to indicate that some text is of strong importance or urgent.

```html
<figcaption>Cats <strong>hate</strong> other cats.</figcaption>
```

![[strong.png]]

### 20

The `form` element is used to get information from a user like their name, email, and other details.

The `action` attribute indicates where form data should be sent.

Here is an example of a `form` element with an `action` attribute:

Example Code

```html
<form action="/submit-url"></form>
```

In the example, `action="/submit-url"` tells the browser that the form data should be sent to the path `/submit-url`.

### 21

The `input` element allows you several ways to collect data from a web form. Like `img` elements, `input` elements are a void element and do not need closing tags.

There are many kinds of inputs you can create using the `type` attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.

### 22

In order for a form's data to be accessed by the location specified in the `action` attribute, you must give the text field a `name` attribute and assign it a value to represent the data being submitted.

Here is an example of an `input` element with a `name` attribute:

Example Code

```html
<input type="text" name="name" />
```

### 23

Placeholder text is used to give people a hint about what kind of information to enter into an input.

Here is an example of an `input` element with a placeholder set to `Ex. Jane Doe`:

Example Code

```html
<input type="text" placeholder="Ex. Jane Doe" />
```
