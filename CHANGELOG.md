# Changelog

All notable changes to the Liquid+ Nova Extension will be documented in this file.

## [1.1.2] - 2025-07-24

### Added

- **JSON + Liquid syntax support** for better mixed-language highlighting
- **Automatic detection** of Liquid code in `.json` files (settings_schema.json, locales, etc.)

### Known Limitations

- JSON sections within `.liquid` files may have highlighting issues after Liquid code appears - this is a Tree-sitter grammar limitation affecting mixed-language parsing

---

## [1.1.1] - 2025-07-18

### Fixes

- Fixed README formatting that was bugging me.

---

## [1.1.0] - 2025-07-18

### Added

- **Auto-completion system** with intelligent bracket handling
- **Liquid tag completions** with smart `%}` closing behavior
- **Shopify object completions** including `product.*`, `collection.*`, `customer.*`, `cart.*`, `settings.*`
- **Complete filter library** with parameter hints for all Liquid and Shopify-specific filters
- **Priority-based completions** offering both simple and full tag completions (e.g., `{% if %}` vs `{% if %}{% endif %}`)
- **Context-aware suggestions** that adapt based on cursor position and existing brackets

### Bug Fixes

- Fixed issue where selecting completions after typing `{%` would result in duplicate closing brackets
- Resolved problem where object completions (like `settings.logo`) wouldn't properly close Liquid tags
- Improved completion consistency across all file types (`.liquid`, `.css.liquid`, `.js.liquid`, `.scss.liquid`)

---
