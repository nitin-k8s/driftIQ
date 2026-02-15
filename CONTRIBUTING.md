# Contributing to DriftIQ

Thank you for your interest in contributing to DriftIQ! This document provides guidelines and instructions for contributing.

## How to Contribute

### Reporting Bugs

If you find a bug, please open an issue with:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable
- Browser and version information

### Suggesting Features

Feature requests are welcome! Please:
- Check if the feature already exists or is planned
- Clearly describe the use case
- Explain how it would benefit users
- Provide examples if possible

### Pull Requests

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/driftiq.git
   cd driftiq
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Keep changes focused and atomic
   - Follow existing code style
   - Test thoroughly in multiple browsers
   - Update documentation if needed

4. **Test your changes**
   - Load example files
   - Test all features
   - Verify export functionality
   - Check localStorage persistence

5. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add: brief description of changes"
   ```

6. **Push and create PR**
   ```bash
   git push origin feature/your-feature-name
   ```
   Then open a Pull Request on GitHub

## Code Style Guidelines

### JavaScript
- Use ES6+ features
- Use `const` and `let`, avoid `var`
- Use template literals for strings
- Add comments for complex logic
- Keep functions focused and small

### HTML/CSS
- Use semantic HTML
- Keep CSS organized by section
- Use CSS variables for colors
- Mobile-responsive design
- Follow existing naming conventions

### Documentation
- Update README.md for new features
- Add inline comments for complex code
- Document API changes
- Include usage examples

## Testing Checklist

Before submitting a PR, verify:
- [ ] Works in Chrome, Firefox, Edge, Safari
- [ ] File loading works correctly
- [ ] Diff computation is accurate
- [ ] Pattern replacement works
- [ ] Ignore rules function properly
- [ ] Export generates valid HTML
- [ ] No console errors
- [ ] localStorage persists correctly
- [ ] Mobile responsive (if UI changes)

## Feature Ideas

Looking for something to work on? Here are some ideas:

### Easy
- Add more example configuration files
- Improve error messages
- Add keyboard shortcuts
- Enhance tooltips

### Medium
- Add diff statistics (lines added/removed/changed)
- Support for multiple file formats
- Dark mode theme
- Command search/filter
- Undo/redo for rules

### Advanced
- Side-by-side text editor mode
- API for programmatic access
- Plugin system for custom parsers
- Batch file comparison
- Git integration

## Community

- Be respectful and constructive
- Help others with issues
- Share your use cases
- Spread the word if you find it useful!

## Questions?

Feel free to open an issue for:
- Questions about contributing
- Help with development setup
- Feature discussions
- General feedback

---

Thank you for contributing to DriftIQ! 🎉
