# Agent Guidelines for deadbeef VSCode Extension

## Build/Test Commands
- No build/test scripts in package.json - this is a theme-only extension
- Use `code --extensionDevelopmentPath=${workspaceFolder}` to test the extension
- Or use VS Code debugger with F5 (launch configuration provided in .vscode/launch.json)

## Code Style Guidelines
- **File Types**: JSON theme files, minimal JavaScript/TypeScript if needed
- **Formatting**: Use proper JSON formatting with consistent indentation (tabs)
- **Colors**: Hex color codes in lowercase (e.g., "#292d3e", "#fce8c3")
- **Naming**: Use descriptive camelCase for properties, kebab-case for CSS-like values
- **Theme Structure**: Follow VS Code theme schema with "colors" and "tokenColors" sections
- **Scope Targeting**: Use specific TextMate scopes for syntax highlighting
- **Color Consistency**: Maintain color palette consistency across all theme elements
- **Comments**: Minimal comments in JSON files, descriptive comments in any code files
- **Error Handling**: N/A for theme files, standard practices for any scripts
- **Imports**: Use relative paths for local assets, absolute for external resources

## Extension Development
- Extension contributes a single dark theme for C/C++, Rust, and Python
- Icon located at `icons/deadbeef-vsc-icon.png`
- Theme definition in `themes/deadbeef-color-theme.json`
- Follow VS Code extension manifest guidelines in package.json
- Test changes by reloading the extension development host window