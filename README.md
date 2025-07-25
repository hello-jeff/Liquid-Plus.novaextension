# Liquid+ Nova Extension

Liquid syntax highlighting for [Panic Nova](https://nova.app) with support for CSS, JavaScript, and SCSS Liquid templates.

## Features

- **Full Liquid syntax highlighting** - All standard Liquid tags, filters, and variables
- **Completions for Tags, Objects, and Filters** - Work in Progress
- **`.css.liquid` file support**
- **`.js.liquid` file support**
- **`.scss.liquid` file support**
- **`.liquid` file support**
- **Built with Tree Sitter**

## Requirements

- **Nova 12.0+** (Tree-sitter support required)

## Configuration

The extension works out of the box with no configuration required. Simply open any `.css.liquid`, `.js.liquid`, or `.scss.liquid` file and enjoy enhanced syntax highlighting.

## Known Issues

- Some complex nested Liquid structures in CSS comments may not highlight perfectly
- SCSS mixins with Liquid variables may show minor highlighting quirks
- JSON sections within `.liquid` files may have highlighting issues after Liquid code appears - this is a Tree-sitter grammar limitation affecting mixed-language parsing

Please report any issues on [GitHub](https://github.com/hello-jeff/Liquid-Plus.novaextension/issues).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Credits

This extension builds upon the excellent work of:

- **[arthrfrts/Liquid.novaextension](https://github.com/arthrfrts/Liquid.novaextension)** - Original Liquid extension for Nova that provided the foundation and Tree-sitter integration
- **[hankthetank27/tree-sitter-liquid](https://github.com/hankthetank27/tree-sitter-liquid)** - The Tree-sitter grammar that powers Liquid syntax parsing

## License

MIT License - see file for details.
