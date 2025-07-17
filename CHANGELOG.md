# Changelog

All notable changes to the Liquid+ Nova Extension will be documented in this file.

## [1.0.0] - 2025-07-16

### Added

- Initial release of Liquid+ extension
- **New file type support:**
  - `.css.liquid` files with CSS + Liquid syntax highlighting
  - `.js.liquid` files with JavaScript + Liquid syntax highlighting
  - `.scss.liquid` files with SCSS + Liquid syntax highlighting
- Enhanced Tree-sitter injection system for mixed-language templates
- Funding support via Buy Me A Coffee

### Enhanced

- Extended base Liquid functionality with multi-language template support
- Improved file detection for Shopify theme development workflows
- Updated extension metadata and configuration

### Technical

- Added new syntax definition files (Liquid-CSS.xml, Liquid-JavaScript.xml, Liquid-SCSS.xml)
- Created injection files for proper language highlighting (css.scm, javascript.scm, scss.scm)
- Updated main.js to register new syntax variants
- Enhanced extension.json with comprehensive activation events

---

## Foundation

This extension is built upon the excellent foundation provided by [arthrfrts/Liquid.novaextension](https://github.com/arthrfrts/Liquid.novaextension), which brought Liquid syntax highlighting to Nova using [hankthetank27's tree-sitter-liquid grammar](https://github.com/hankthetank27/tree-sitter-liquid).

**Original Extension Changelog:** For the history of the base Liquid extension that this builds upon, see the [original changelog](https://github.com/arthrfrts/Liquid.novaextension/blob/main/CHANGELOG.md).

---

## Contributing

Found a bug or have a feature request? Please [open an issue](https://github.com/hello-jeff/Liquid-Plus.novaextension/issues) or submit a pull request.

## Support

If you find this extension helpful, consider [buying me a coffee](https://coff.ee/hellojeff) ☕️
