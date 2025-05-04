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
In the previous step, you put the `h1`, `h2`, comment, and `p` elements inside the `main` element. This is called _nesting_. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.

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
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg">
```

### 9
All `img` elements should have an `alt` attribute. The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

Here is an example of an `img` element with an `alt` attribute:

Example Code

```html
<img src="cat.jpg" alt="A cat">
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
  <img src="image-link.jpg" alt="A photo of a cat.">
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
  <img src="image.jpg" alt="A description of the image">
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
<input type="text" name="name">
```

### 23
Placeholder text is used to give people a hint about what kind of information to enter into an input.

Here is an example of an `input` element with a placeholder set to `Ex. Jane Doe`:

Example Code

```html
<input type="text" placeholder="Ex. Jane Doe">
```

### 24
To prevent a user from submitting your form when required information is missing, you need to add the `required` attribute to an `input` element.

Here is an example of an input field with the `required` attribute:

Example Code

```html
<input type="text" name="firstName" required>
```

There's no need to set a value to the `required` attribute. Instead, just add the word `required` to the `input` element, making sure there is space between it and other attributes.

### 25
The `button` element is used to create a clickable button.

Add a `button` element with the text `Submit` below the `input` element. The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's `action` attribute.

### 26
Even though you added your button below the text input, they appear next to each other on the page. That's because both `input` and `button` elements are inline elements, which don't appear on new lines.

The button you added will submit the form by default. However, relying on default behavior may cause confusion. Add the `type` attribute with the value `submit` to the `button` to make it clear that it is a submit button.

### 27
You can use radio buttons for questions where you want only one answer out of multiple options.

Here is an example of a radio button with the text set as `cat`:

Example Code

```html
<input type="radio"> cat
```

Remember that an `input` element is a void element.

### 28
`label` elements are used to help associate the text for an `input` element with the `input` element itself (especially for assistive technologies like screen readers).

Here is an example of a `label` element with a `radio` button:

Example Code

```html
<label><input type="radio"> cat</label>
```

In the example, clicking on the word `"cat"` will also select the `radio` button.

Nest your `radio` button inside a `label` element.

### 29
The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other `id` values for the entire page.

Here is an example of an `input` element with an `id` attribute:

Example Code

```html
<input id="email">
```

### 30
Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a `name` attribute with the same value.

Here is an example of two radio buttons with the same `name` attribute:

Example Code

```html
<input type="radio" name="meal"> Breakfast
<input type="radio" name="meal"> Lunch
```

Add the `name` attribute with the value `indoor-outdoor` to both radio buttons.

### 31
If you select the `Indoor` radio button and submit the form, the form data for the button is based on its `name` and `value` attributes. Since your radio buttons do not have a `value` attribute, the form data will include `indoor-outdoor=on`, which is not useful when you have multiple buttons.

Add a `value` attribute to both radio buttons. For convenience, set the button's `value` attribute to the same value as its `id` attribute.

### 32
The `fieldset` element is used to group related inputs and labels together in a web form. `fieldset` elements are block-level elements, meaning that they appear on a new line.

Nest the `Indoor` and `Outdoor` radio buttons within a `fieldset` element, and don't forget to indent the radio buttons.
```html
<fieldset>
	<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
	<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```

### 33
The `legend` element acts as a caption for the content in the `fieldset` element. It gives users context about what they should enter into that part of the form.

Add a `legend` element with the text `Is your cat an indoor or outdoor cat?` above both of the radio buttons.
```html
<fieldset>
	<legend>Is your cat an indoor or outdoor cat?</legend>
	<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
	<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```

### 34
Forms commonly use checkboxes for questions that may have more than one answer. The `input` element with a `type` attribute set to `checkbox` creates a checkbox.

### 35
There's another way to associate an `input` element's text with the element itself. You can nest the text within a `label` element and add a `for` attribute with the same value as the `input` element's `id` attribute.

Given an `input` element as below:

Example Code

```html
<input id="breakfast" type="radio" name="meal" value="breakfast">
```

An example of a `label` element that is associated to this `input` element is:

Example Code

```html
<label for="breakfast">Breakfast</label>
```

### 36
While the `value` attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.

### 37
In order to make a checkbox checked or radio button selected by default, you need to add the `checked` attribute to it.

Here is an example of a radio button with the `checked` attribute:

Example Code

```html
<input checked type="radio" name="meal" value="breakfast"> Breakfast
```

There's no need to set a value to the `checked` attribute. Instead, just add the word `checked` to the `input` element, making sure there is space between it and other attributes.

Make the first radio button and the first checkbox selected by default.

### 38
The `footer` element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.

After the `main` element, add a `footer` element.

### 39
Notice that everything you've added to the page so far is inside the `body` element. All page content elements that should be rendered to the page go inside the `body` element. However, other important information goes inside the `head` element.

The `head` element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.

 `head` element added above the `body` element.

### 40
The `title` element determines what browsers show in the title bar or tab for the page.

### 41
Notice that the entire contents of the page are nested within an `html` element. The `html` element is the root element of an HTML page and wraps all content on the page.

You can also specify the language of your page by adding the `lang` attribute to the `html` element.

Add the `lang` attribute with the value `en` to the opening `html` tag to specify that the language of the page is English.

### 42
All pages should begin with `<!DOCTYPE html>`. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.

`<!DOCTYPE html>` tells browsers that the document is an HTML5 document which is the latest version of HTML.

### 43
You can set browser behavior by adding `meta` elements in the `head`. Here's an example:

Example Code

```html
<meta attribute="value">
```

Inside the `head` element, nest a `meta` element with an attribute named `charset`. Set to the value to `utf-8` which tells the browser how to encode characters for the page.

Note that the `meta` element is a void element.

`index.html`
```html
<!DOCTYPE html>

  

<html lang="en">

  <head>

    <meta charset="utf-8">

    <title>CatPhotoApp</title>

  </head>

  <body>

    <main>

      <h1>CatPhotoApp</h1>

      <section>

        <h2>Cat Photos</h2>

        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>

        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>

        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>

      </section>

      <section>

        <h2>Cat Lists</h2>

        <h3>Things cats love:</h3>

        <ul>

          <li>catnip</li>

          <li>laser pointers</li>

          <li>lasagna</li>

        </ul>

        <figure>

          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">

          <figcaption>Cats <em>love</em> lasagna.</figcaption>  

        </figure>

        <h3>Top 3 things cats hate:</h3>

        <ol>

          <li>flea treatment</li>

          <li>thunder</li>

          <li>other cats</li>

        </ol>

        <figure>

          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">

          <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  

        </figure>

      </section>

      <section>

        <h2>Cat Form</h2>

        <form action="https://freecatphotoapp.com/submit-cat-photo">

          <fieldset>

            <legend>Is your cat an indoor or outdoor cat?</legend>

            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>

            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>

          </fieldset>

          <fieldset>

            <legend>What's your cat's personality?</legend>

            <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>

            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>

            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>

          </fieldset>

          <input type="text" name="catphotourl" placeholder="cat photo URL" required>

          <button type="submit">Submit</button>

        </form>

      </section>

    </main>

    <footer>

      <p>

        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>

      </p>

    </footer>

  </body>

</html>
```