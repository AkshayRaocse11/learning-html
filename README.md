# Understanding Quirks Mode in Web Browsers

In the early days of the web, pages were often created in two versions: one for Netscape Navigator and one for Microsoft Internet Explorer. When web standards were introduced by the W3C, browsers couldn't immediately adopt them without breaking most existing sites. To address this, browsers introduced two modes to differentiate between new standards-compliant sites and legacy sites.

## Browser Modes

Modern browsers utilize three different modes:

1. **Quirks Mode**: Emulates behavior found in older browsers like Netscape Navigator 4 and Internet Explorer 5. This mode is essential for supporting websites built before the widespread adoption of web standards.

2. **Limited-Quirks Mode** (previously known as "Almost Standards" Mode): Implements only a few quirks.

3. **No-Quirks Mode** (previously known as "Full Standards" Mode): The layout and behavior adhere to modern HTML and CSS specifications.

## Determining Browser Mode

For HTML documents, the browser uses the DOCTYPE declaration at the beginning of the document to decide whether to render the page in quirks mode or standards mode.

### Example of DOCTYPE for Standards Mode

To ensure your page uses no-quirks mode, include the following DOCTYPE at the beginning of your HTML document:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Hello World!</title>
  </head>
  <body></body>
</html>

#### <head>
Nested between the opening and closing <html> tags, we find the two children: <head> and <body>:

<!DOCTYPE html>
<html lang="en-US">
  <head>
  </head>
  <body>
  </body>
</html>

