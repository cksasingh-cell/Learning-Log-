# Contributing to Learning-Log

First off, thank you for considering contributing to Learning-Log! It's people like you that make Learning-Log such a great tool.

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [your-email@example.com].

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When you create a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples** to demonstrate the steps
- **Describe the behavior you observed** and what you expected
- **Include screenshots** if possible
- **Specify browser and version** (especially important for voice recognition issues)
- **Note if the problem is Hindi or English specific**

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description** of the suggested enhancement
- **Explain why this enhancement would be useful**
- **List some examples** of how it would be used
- **Include mockups or examples** if applicable

### Pull Requests

1. **Fork the repo** and create your branch from `main`
2. **Make your changes** following our coding standards
3. **Test thoroughly** in multiple browsers (especially Chrome for Hindi)
4. **Update documentation** if needed
5. **Write clear commit messages**
6. **Submit a pull request**

#### Pull Request Guidelines

- Keep PRs focused on a single feature/fix
- Update README.md if adding new features
- Test Hindi and English voice recognition if touching that code
- Test on mobile if changing responsive design
- Follow the existing code style
- Write meaningful commit messages

## Development Setup

1. Clone your fork:
   ```bash
   git clone https://github.com/your-username/learning-log.git
   cd learning-log
   ```

2. Open `index.html` in your browser or run a local server:
   ```bash
   python -m http.server 8000
   ```

3. Make your changes and test in:
   - Chrome (for Hindi voice)
   - Firefox
   - Safari
   - Mobile browsers

## Coding Standards

### JavaScript
- Use ES6+ features
- Use meaningful variable names
- Add comments for complex logic
- Keep functions small and focused
- Handle errors gracefully

### CSS
- Use consistent naming conventions
- Keep specificity low
- Use CSS variables for colors
- Maintain responsive design principles
- Test animations on different devices

### HTML
- Use semantic HTML5 elements
- Maintain accessibility standards
- Keep structure clean and readable

## Testing Guidelines

Before submitting a PR, please test:

1. **Voice Recording**
   - English voice recognition works
   - Hindi voice recognition works (Chrome)
   - Pause/Resume functionality
   - Timer accuracy
   - Transcription appears correctly

2. **Manual Typing**
   - English typing
   - Hindi typing (with Hindi keyboard)
   - Character count updates
   - Auto-save works

3. **Note Management**
   - Create, edit, delete notes
   - Search functionality
   - Sort by newest/oldest
   - Expand/collapse works

4. **Book Management**
   - Add, edit, delete books
   - Note count updates
   - Selection works

5. **PDF Export**
   - All notes appear in PDF
   - Hindi text renders correctly
   - Formatting looks good
   - Print dialog opens

6. **Responsive Design**
   - Works on mobile (< 768px)
   - Works on tablet
   - Works on desktop
   - Sidebar behavior on mobile

7. **Data Persistence**
   - Data saves to localStorage
   - Data loads on refresh
   - Language preference persists

## Priority Areas for Contribution

We especially welcome contributions in these areas:

1. **More Language Support**
   - Spanish, French, German, etc.
   - RTL languages (Arabic, Hebrew)

2. **Cloud Integration**
   - Google Drive sync
   - Dropbox integration
   - OneDrive support

3. **Export Formats**
   - Export to Word (.docx)
   - Export to Markdown
   - Export to plain text

4. **Features**
   - Dark mode
   - Tags/categories for notes
   - Note templates
   - Bulk operations

5. **Mobile Apps**
   - React Native app
   - Progressive Web App (PWA)

6. **Accessibility**
   - Screen reader support
   - Keyboard navigation improvements
   - High contrast mode

## Questions?

Feel free to open an issue with the `question` label if you have any questions about contributing!

## Recognition

Contributors will be recognized in the README.md file.

Thank you for contributing! 🙏
