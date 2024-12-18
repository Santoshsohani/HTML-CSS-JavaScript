
## Why `index.html` is first loaded

The `index.html` file is served first by the web server and acts as the entry point for the application. Most web servers are pre-configured to load the `index.html` file by default when no specific file name is provided in the URL.

When a user enters a URL without specifying a file, the server automatically delivers the `index.html` file. This file typically references other resources such as images, icons, CSS, and JavaScript, which are loaded by the browser to render the web page.

## Structure of HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
</html>
```

- **`<!DOCTYPE html>`**: Previously, multiple doctypes like XML and XHTML were used. This tag specifies the type of document being used, helping the browser render the content correctly.
- **`<html>`**: Acts as the root element of the document, containing all essential information and the complete content of the webpage.
- **`<head>`**: Contains crucial details about the document, such as the title, metadata, and favicons.
- **`<body>`**: Holds the main content of the webpage, comprising various nested tags that structure the page layout.

## Importance of Tags wrt SEO

HTML tags play a vital role in **SEO (Search Engine Optimization)** because they help search engines understand the structure, content, and relevance of a web page. Proper usage of these tags can improve search engine rankings, user engagement, and website accessibility.

Here’s why various HTML tags are important for SEO:

1. **`<title>`**: Defines the page title; crucial for search engine rankings and click-through rates from SERPs.
2. **`<meta>`**: Provides metadata (e.g., description, keywords) that helps search engines understand the page content.
3. **`<h1>` to `<h6>`**: Structure the content; makes it easier for search engines to determine the hierarchy and relevance of the content.
4. **`<a>` (Anchor)**: Enables linking to other pages, improving navigation, link equity distribution, and site authority.
5. **`<img>`**: Optimized `alt` attributes improve accessibility and help search engines understand and rank images.
6. **`<strong>` and `<em>`**: Add emphasis to important text, making it more prominent for search engines.
7. **Lists (`<ul>`, `<ol>`, `<li>`)**: Enhance readability and help search engines feature content in rich snippets.
8. **`<header>` and `<footer>`**: Organize the site layout, improving crawlability and user experience.
9. **`<article>` and `<section>`**: Provide semantic meaning, improving content ranking for specific topics.
10. **`<nav>`**: Improves site structure, aiding search engine crawling and user navigation.


## Documentation to follow
[MDN DOCS](https://developer.mozilla.org/en-US/)

## Different color formats

### Hexadecimal
- It is a 6 character color format
- Uses base-16 system which lies between 0-9 and A-F
- #RRGGBB or #RRGGBBAA
	- R - red
	- G - green
	- B - blue
	- A - alpha (transparency)

### RGB 
- It uses numbers between 0-255
- Mixing of colors (RED, GREEN, BLUE) to get the desired color output.
- example : rgb(255,0,0)
- There is also another associated format rgba(0,255,128,0.4)

### HSL (Hue, Saturation, Lightness)
- H - Position on the color wheel (Degree)
- S - Intensity of the color (Percentage)
- L - Lightness of the color (Percentage)

`hsl(14, 100%, 60%)` → Orange
`hsla(240, 100%, 50%, 0.7)` → Blue with 70% transparency

## BDO: Bi-Directional Override
It is the tag which is used to specify the content to display either from right-left or left-right.

```html
<bdo dir="ltr">Text content</bdo>
<bdo dir="rtl">Text content</bdo>
```

The `<bdo>` tag is supported in all major browsers:

- Chrome
- Firefox
- Safari
- Edge
- Opera

## Anchor Tags

The `target` attribute of the `<a>` (anchor) tag specifies where to open the linked document.  
There are widely two values used with it:   
- _self_  
- _target_

The `_self` value to the attribute opens the linked document in the same tab itself, where as the `_target` opens it in new tab.

```html  
<a href="https://example.com" target="_self">Same Tab</a>  
<a href="https://example.com" target="_self">New Tab</a>  
```

## Address Tag

The `<address>` element is used when the content to be displayed is contact information, address or any other such details is written under the `<address>` tag.  

The `<address>` tag can be nested with the same `<address>` tag but not with the other tags such as `<div> <header>`

```html  
<address>  
  You can contact author at  
<a href="[http://www.example.com/contact">www.example.com</a>.<br](http://www.example.com/contact%22>www.example.com</a>.<br "http://www.example.com/contact%22%3ewww.example.com%3c/a%3e.%3cbr") />  
  If you see any bugs, please  
<a href="mailto:webmaster@example.com">contact webmaster</a>.<br />  
  You may also want to visit us:<br />  
  Mozilla Foundation<br />  
  331 E Evelyn Ave<br />  
  Mountain View, CA 94041<br />  
  USA  
</address>  
```

## Global Attributes

Global attributes are the once which are available to all the elements apart from their individual attributes (if any). Some of the global attributes are :   
1. class  
2. id  
3. style

## Class and Id

In HTML, **class** and **id** attributes are used to uniquely identify and target elements for various operations, such as styling with CSS or manipulating them using JavaScript and the DOM.

### Key Rules and Differences:

1. A single page can have **multiple elements** with the same class name.
    
    - Classes are generally used when you need to apply the same styles or functionality to a group of elements.
2. A single page can have **multiple id attributes**, but each id must be **unique** to one element.
    
    - Ids are used to target **specific, unique elements**.

### Why This Distinction Exists:

- The **id** attribute is intended to uniquely identify a single element for precise operations, such as JavaScript manipulation.
- The **class** attribute is meant for grouping elements to apply common styles or behaviors.

Previously, the JavaScript community decided that using **ids** for targeting single elements was more efficient, as browsers optimize the `getElementById` method for performance. For grouping or shared operations, **classes** are more appropriate.

## iframe

`iframe` is an inline element which is used to embed other html document within another document.

```html
<iframe
  id="inlineFrameExample"
  title="Inline Frame Example"
  width="300"
  height="200"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik">
</iframe>
```

### Attributes 
1. `allow` : It is the attribute which is used to control the permissions for the content present in the `iframe` such as `autoplay payment fullscreen`
2. `height`
3. `width`
4. `loading` : eager (default) or lazy loading


## Head 

The `<head>` tag in an HTML page contains meta-information about the page. This includes the title, styling, and other metadata that helps define the page's behavior and appearance.

### Example:

```html
<meta charset="UTF-8">
```

- The `charset` attribute specifies the character encoding for the document.
- **UTF-8** is the most commonly used character encoding because it supports a wide range of characters, including those from multiple languages (like Japanese, Spanish, etc.) and symbols like emojis.
- **UTF-16** is rarely used in web development today, as UTF-8 is more efficient and widely supported, even for multi-language pages.

---

### Another Example:

```html
<meta name="" content="">
```

- This is the **basic syntax** for a `<meta>` tag.
- The `name` attribute specifies the type of meta-information (e.g., description, viewport).
- The `content` attribute provides the value for the specified `name`.

---

### Meta Tag for Responsive Design:

One commonly used meta tag adjusts the zoom level and layout based on the device's screen width:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- **`width=device-width`**: Makes the page width match the device's screen width.
- **`initial-scale=1.0`**: Sets the initial zoom level to 100%.

This tag ensures your page is mobile-friendly and responsive.
