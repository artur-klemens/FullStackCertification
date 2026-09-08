# Full Stack Development Notes

## HTML Basics

- HTML is written using elements.
- `<h1></h1>` is the main heading of a webpage, and you should only use one per page.
- `<h2>` represent subheadings, and you can have multiple on a page.
- There are six heading elements in HTML (h1 through h6).
- HTML represents the content and structure of a webpage. JavaScript adds interactivity to a webpage (fonts, colors, etc.), and JavaScript adds interactivity to a webpage.
- Some HTML elements don't have a closing tag; these are called "void elements" and an example is `<img>` or `<img />`
- The div element is used for grouping HTML elements, mainly when you want them to share the same CSS style
- "id" is an attribute than can add a unique identifier to every element, which can then be referenced in "Javascript" or "CSS"
- "id"s should be unique and not reused; to target multiple elements: add the "class" attribute to them; to target a specific element: add "id"
- To represent reserved characters (ex: < or >) in HTML, you must use entities (or character references; ex: &lt; &gt;). These two are named character references; decimal character references start with "&#" followed by 1 or more digits; hexadecimal character references start with "&x" followed by 1 or more ASCII hex digits. All of them end with ";"

## Links and External Resources

- The link element is used to link to external resources (e.g. stylesheets and site icons). It is common practice to keep HTML and CSS in separate files. Example: `<link rel="stylesheet" href="./styles.css" />`
- The link element must be placed inside the head element, and can also link to external URLs (ex. Google Fonts). In this case, the rel attribute should have the "preconnect" value, to make loading faster.
- You should have an HTML boilerplate that contains the essential foundation for creating an HTML file.
- The "script" element is used to embed executable code (Javascript). Example usage: "<script src="path-to-javascript-file.js"></script>"; it is best practice to link a script file there instead of writing it in the HTML document itself.

## Semantic HTML

- HTML has some elements that identify different content areas, and this helps with SEO. main is such an element.
- section is another element that helps to define sections in an HTML document.
- section is used to define chapters, headers, footers, or any other sections in a document.
- When you add a lower-rank heading to the doc, it's implied that you're starting a new subsection.
- figure represents self-contained content, and allows you to add captions to images. "ul" is used for creating an unordered list (list elements are defined with "li").
- You add a caption to a figure with "figcaption".
- "strong" and "em" are used for bold and italic.
- "footer" is used to define a footer - usually contains info about the author, copyright data, ToS, contact info, etc.
- "div" should not be overused, because it has no semantic meaning; ex. "section" means one thing explicitly, and browsers know what to do when encountering this element