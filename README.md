# Static-Site
Static Site Project
This will become a blog

## What this code will do
1. Delete everything in the /public directory.
2. Copy any static assets (HTML template, images, CSS, etc.) to the /public directory.
3. Generate an HTML file for each Markdown file in the /content directory. For each Markdown file:
4. Open the file and read its contents.
5. Split the markdown into "blocks" (e.g., paragraphs, headings, lists, etc.).
6. Convert each block into a tree of HTMLNode objects. For inline elements (like bold text, links, etc.), we will convert:
7. Raw markdown -> TextNode -> HTMLNode
8. Join all the HTMLNode blocks under one large parent HTMLNode for the pages.
9. Use a recursive to_html() method to convert the HTMLNode and all its nested nodes to a giant HTML string and inject it into the HTML template.
10. Write the full HTML string to a file for that page in the /public directory.
