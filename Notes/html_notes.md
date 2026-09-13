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
- You can add audio and video elements to an HTML page using `audio` and `video`

## Links and External Resources

- The link element is used to link to external resources (e.g. stylesheets and site icons). It is common practice to keep HTML and CSS in separate files. Example: `<link rel="stylesheet" href="./styles.css" />`
- The link element must be placed inside the head element, and can also link to external URLs (ex. Google Fonts). In this case, the rel attribute should have the "preconnect" value, to make loading faster.
- The target attribute on anchor / link elements determine where the page opens; \_self = current browsing context; \_blank = new context (e.g. new tab); \_parent = in parent of the current context; \_top = top-most context
- Links can have five different states: `:link`, the default (unclicked) state; `:visited`;`:hover`; `:focus` when the link is focused using Tab; `:active` when clicked; the order listed here is also the order that must be specified in CSS
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

## Audio and Video

- The `audio` element can have different attributes that control how it behaves: `src` for providing the audio file, `loop` to control if the audio loops (`loop` is a bool and doesn’t need a value)
- The `controls` attribute in `audio` is also a bool that provides the user with controls to play/stop the media file.
- The `video` element has a `width` attribute
- The `video` element also has the bool attributes `loop` and `controls`
- Both `audio` and `video` elements have the `muted` attribute, to control if the media is muted when the first playback starts

## Video Formats

- When it comes to `video` format support, it is browser dependent; so you need to provide multiple types of video, that the browser can select. The syntax is:

```html
  <source src="src-url-goes-here" type="video-type-goes-here" />
```

- Media types must be specified using a MIME format (ex. `video/mp4`)
- All the popular video format types are: `video/mp4` `video/webm` `video/ogg` and `video/quicktime`

## Iframes

- iframes are replaced elements; replaced elements are elements whose contents are determined by an external source, rather than CSS (e.g. website, image, embedded video)
- iframe can also be used to embed another HTML page directly
- When embedding a video, the `allow` attribute defines an allowlist of features that the embedded content is allowed to use (e.g. autoplay, accelerometer, clipboard-write)

## Media Considerations

- When using media, you should consider: size, format and compression\

## Images

- Image formats for older browsers: PNG, JPEG; more modern formats: WEBP, AVIF
- Images on the web are by default released under “All Rights Reserved”; use tools like Unsplash/Pixabay to find images with permissive licenses

## SVG

- SVGs are vector graphics, and they can be defined directly in HTML; they are useful when wanting to have custom icons on your page, e.g. for social media icons
- SVG stores the data in XML format
