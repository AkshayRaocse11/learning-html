#Learning Html
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

## Content Language

The `lang` attribute in the `<html>` tag defines the main language of the document using a two- or three-letter ISO language code, optionally followed by a region code (e.g., `fr-CA` for Canadian French). This attribute helps screen readers, search engines, and translation services determine the document's language.

### Usage of `lang` Attribute

- **Global Language Declaration**: Place the `lang` attribute in the `<html>` tag to set the language for the entire document.
- **Localized Language Exceptions**: Use the `lang` attribute within the body to specify parts of the document that differ from the main language.
- **No Visual Impact**: The `lang` attribute is purely semantic, providing information to assistive technologies without affecting the document's appearance.

### CSS Selectors and `lang`

The `lang` attribute can also be utilized in CSS selectors. For instance, `<span lang="fr-fr">Ceci n'est pas une pipe.</span>` can be targeted using `[lang|="fr"]` or `:lang(fr)` in your CSS.
