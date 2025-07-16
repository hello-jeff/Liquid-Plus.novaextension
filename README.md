# Liquid+ Nova Extension

Enhanced Liquid syntax highlighting for [Panic Nova](https://nova.app) with support for CSS, JavaScript, and SCSS Liquid templates.

## Features

✅ **Full Liquid syntax highlighting** - All standard Liquid tags, filters, and variables  
✅ **`.css.liquid` file support** - CSS with embedded Liquid templating  
✅ **`.js.liquid` file support** - JavaScript with embedded Liquid templating  
✅ **`.scss.liquid` file support** - SCSS with embedded Liquid templating  
✅ **`.liquid` file support** - Standard HTML Liquid templates  
✅ **Tree-sitter powered** - Fast, accurate syntax parsing  
✅ **Auto-completion** - Intelligent Liquid tag and filter suggestions  
✅ **Auto-pairing** - Smart bracket and quote completion

## Perfect for Shopify Development

This extension is specifically designed for Shopify theme developers who work with mixed-language Liquid templates:

```css
/* styles.css.liquid */
.header {
  background-color: {{ settings.header_bg_color }};
  font-size: {{ settings.header_font_size }}px;
}

{% if settings.show_border %}
.header {
  border: 1px solid {{ settings.border_color }};
}
{% endif %}
```

```javascript
// script.js.liquid
const productData = {
  id: {{ product.id }},
  title: "{{ product.title | escape }}",
  price: {{ product.price | divided_by: 100.0 }},
  available: {{ product.available | json }}
};

{% if customer %}
const customerInfo = {
  id: {{ customer.id }},
  email: "{{ customer.email | escape }}"
};
{% endif %}
```

## Installation

### From Nova Extension Library

1. Open Nova
2. Go to **Extensions → Extension Library**
3. Search for **"Liquid+"**
4. Click **Install**

### Manual Installation

1. Download the latest release from [GitHub](https://github.com/hello-jeff/Liquid-Plus.novaextension/releases)
2. Double-click the `.novaextension` file
3. Nova will install it automatically

## Supported File Types

| Extension      | Language            | Description                       |
| -------------- | ------------------- | --------------------------------- |
| `.liquid`      | HTML + Liquid       | Standard Liquid templates         |
| `.css.liquid`  | CSS + Liquid        | Stylesheets with Liquid variables |
| `.js.liquid`   | JavaScript + Liquid | Scripts with Liquid data          |
| `.scss.liquid` | SCSS + Liquid       | Sass stylesheets with Liquid      |
| `.html.liquid` | HTML + Liquid       | HTML templates with Liquid        |

## What's New in Liquid+

This extension enhances the original Liquid extension with support for mixed-language templates that are common in Shopify development but weren't previously supported in Nova:

- **CSS Liquid Templates** - Style files that use Liquid for dynamic theming
- **JavaScript Liquid Templates** - Script files that embed Liquid data
- **SCSS Liquid Templates** - Sass files with Liquid variable injection
- **Enhanced Tree-sitter Integration** - Improved parsing for complex mixed-language files

## Requirements

- **Nova 4.0+** (Tree-sitter support required)
- **macOS 10.15+**

## Configuration

The extension works out of the box with no configuration required. Simply open any `.css.liquid`, `.js.liquid`, or `.scss.liquid` file and enjoy enhanced syntax highlighting.

## Known Issues

- Some complex nested Liquid structures in CSS comments may not highlight perfectly
- SCSS mixins with Liquid variables may show minor highlighting quirks

Please report any issues on [GitHub](https://github.com/hello-jeff/Liquid-Plus.novaextension/issues).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Credits

This extension builds upon the excellent work of:

- **[arthrfrts/Liquid.novaextension](https://github.com/arthrfrts/Liquid.novaextension)** - Original Liquid extension for Nova that provided the foundation and Tree-sitter integration
- **[hankthetank27/tree-sitter-liquid](https://github.com/hankthetank27/tree-sitter-liquid)** - The Tree-sitter grammar that powers Liquid syntax parsing
- **[Shopify](https://shopify.github.io/liquid/)** - For creating the Liquid templating language

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Support

- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/hello-jeff/Liquid-Plus.novaextension/issues)
- 💡 **Feature Requests**: [GitHub Issues](https://github.com/hello-jeff/Liquid-Plus.novaextension/issues)
- 📧 **Contact**: [hello@jeffdashley.com](mailto:hello@jeffdashley.com)

---

**Made with ❤️ for the Shopify development community**
