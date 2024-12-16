
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



