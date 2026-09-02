# Full Stack Development Notes

## HTML Basics

- The div element is used for grouping HTML elements, mainly when you want them to share the same CSS style
- "id" is an attribute than can add a unique identifier to every element, which can then be referenced in "Javascript" or "CSS"
- "id"s should be unique and not reused; to target multiple elements: add the "class" attribute to them; to target a specific element: add "id"
- To represent reserved characters (ex: < or >) in HTML, you must use entities (or character references; ex: &lt; &gt;). These two are named character references; decimal character references start with "&#" followed by 1 or more digits; hexadecimal character references start with "&x" followed by 1 or more ASCII hex digits. All of them end with ";"

## Links and External Resources

- The "script" element is used to embed executable code (Javascript). Example usage: "<script src="path-to-javascript-file.js"></script>"; it is best practice to link a script file there instead of writing it in the HTML document itself.

## Semantic HTML

- "div" should not be overused, because it has no semantic meaning; ex. "section" means one thing explicitly, and browsers know what to do when encountering this element
