# 🌧️ Contributing to Rain for Relax

Thank you for your interest in contributing to Rain for Relax! We welcome all contributions, whether it's bug reports, feature requests, documentation improvements, or code contributions.

## 📋 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [How Can I Contribute?](#-how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
- [Development Setup](#-development-setup)
- [Pull Request Process](#-pull-request-process)
- [Code Style Guide](#-code-style-guide)
- [License](#-license)

## ✨ Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## 🤔 How Can I Contribute?

### Reporting Bugs

- Ensure the bug was not already reported by searching on GitHub under [Issues](https://github.com/isyuricunha/rain-for-relax/issues).
- If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/isyuricunha/rain-for-relax/issues/new). Be sure to include:
  - A clear and descriptive title
  - Steps to reproduce the issue
  - Expected vs. actual behavior
  - Browser and OS version
  - Any relevant screenshots or console output

### Suggesting Enhancements

- Check if the enhancement has already been suggested in the [issues](https://github.com/isyuricunha/rain-for-relax/issues).
- Open a new issue with a clear title and description of the enhancement.
- Explain why this enhancement would be useful to users.
- Include any mockups or examples if applicable.

### Your First Code Contribution

1. Fork the repository on GitHub.
2. Clone your fork locally:
   ```bash
   git clone https://github.com/your-username/rain-for-relax.git
   cd rain-for-relax
   ```
3. Create a new branch for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. Make your changes and commit them with a clear commit message.
5. Push your changes to your fork.
6. Open a pull request against the `main` branch.

## 🛠️ Development Setup

No complex setup is needed! This project uses vanilla HTML, CSS, and JavaScript with no build step.

1. Open `index.html` in your browser to test changes locally.
2. For testing with a local server (optional):
   ```bash
   # Python 3
   python -m http.server 8000
   # or with PHP
   php -S localhost:8000
   ```
3. Open `http://localhost:8000` in your browser.

## 🔄 Pull Request Process

1. Ensure any install or build dependencies are removed before the end of the layer when doing a build.
2. Update the README.md with details of changes to the interface, this includes new environment variables, exposed ports, useful file locations, and container parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this Pull Request would represent. The versioning scheme we use is [SemVer](http://semver.org/).
4. You may merge the Pull Request in once you have the sign-off of one other developer, or if you do not have permission to do that, you may request the reviewer to merge it for you.

## 🎨 Code Style Guide

### HTML
- Use semantic HTML5 elements.
- Use kebab-case for class names.
- Include proper ARIA attributes for accessibility.
- Indent with tabs.

### CSS
- Follow BEM naming convention.
- Use CSS variables for theming.
- Keep styles organized by component.
- Include comments for complex styles.

### JavaScript
- Use modern ES6+ syntax.
- Use meaningful variable and function names.
- Add comments for complex logic.
- Keep functions small and focused on a single responsibility.

## 📜 License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE).

## 🙏 Thanks!

Thank you for taking the time to contribute to Rain for Relax! Your help is greatly appreciated.
