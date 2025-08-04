# Contributing to ALX Frontend Projects

![Contributing](https://img.shields.io/badge/Contributing-Welcome-brightgreen)
![Code Style](https://img.shields.io/badge/Code%20Style-Prettier-ff69b4)
![License](https://img.shields.io/badge/License-Educational-blue)

Thank you for your interest in contributing to the ALX Frontend Development projects! This guide will help you understand our development process and how to contribute effectively.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)
- [Documentation](#documentation)
- [Testing](#testing)

## 🤝 Code of Conduct

We are committed to providing a welcoming and inspiring community for all. Please read and follow our Code of Conduct:

### Our Pledge
- Use welcoming and inclusive language
- Be respectful of differing viewpoints and experiences
- Gracefully accept constructive criticism
- Focus on what is best for the community
- Show empathy towards other community members

### Our Standards
**Positive behavior includes:**
- Demonstrating empathy and kindness
- Being respectful of differing opinions
- Giving and gracefully accepting constructive feedback
- Taking responsibility for our mistakes
- Focusing on what is best for the overall community

**Unacceptable behavior includes:**
- Trolling, insulting comments, and personal attacks
- Public or private harassment
- Publishing others' private information without permission
- Other conduct which could reasonably be considered inappropriate

## 🚀 Getting Started

### Prerequisites

Before contributing, ensure you have:

- **Git** installed and configured
- **Modern web browser** (Chrome, Firefox, Safari, Edge)
- **Text editor** or IDE (VS Code recommended)
- **Basic knowledge** of HTML5, CSS3, and web standards
- **Understanding** of responsive design principles

### Setting Up Your Development Environment

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/your-username/alx-frontend.git
   cd alx-frontend
   ```

3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/salmaneben/alx-frontend.git
   ```

4. **Verify your setup**
   ```bash
   git remote -v
   # Should show both origin (your fork) and upstream (original repo)
   ```

### Recommended VS Code Extensions

Install these extensions for the best development experience:

```json
{
  "recommendations": [
    "bradlc.vscode-tailwindcss",
    "stylelint.vscode-stylelint",
    "formulahendry.auto-rename-tag",
    "christian-kohler.path-intellisense",
    "ms-vscode.vscode-html-languageservice",
    "zignd.html-css-class-completion",
    "esbenp.prettier-vscode",
    "ritwickdey.liveserver"
  ]
}
```

## 🔄 Development Workflow

### Branch Naming Convention

Use descriptive branch names that follow this pattern:

```bash
# Feature branches
feature/add-navigation-menu
feature/implement-dark-theme
feature/responsive-grid-system

# Bug fix branches
fix/header-alignment-issue
fix/mobile-navigation-bug
fix/accessibility-contrast

# Documentation branches
docs/update-readme
docs/add-contributing-guide
docs/api-documentation

# Refactoring branches
refactor/css-architecture
refactor/html-semantic-structure
```

### Creating a Feature Branch

```bash
# Ensure you're on the main branch and it's up to date
git checkout main
git pull upstream main

# Create and switch to a new feature branch
git checkout -b feature/your-feature-name

# Make your changes and commit them
git add .
git commit -m "Add your descriptive commit message"

# Push to your fork
git push origin feature/your-feature-name
```

## 📝 Coding Standards

### HTML Guidelines

#### Semantic Structure
```html
<!-- ✅ Good: Use semantic HTML5 elements -->
<article class="blog-post">
  <header class="blog-post__header">
    <h1 class="blog-post__title">Article Title</h1>
    <time class="blog-post__date" datetime="2023-01-01">January 1, 2023</time>
  </header>
  <section class="blog-post__content">
    <p>Article content goes here...</p>
  </section>
</article>

<!-- ❌ Avoid: Generic div soup -->
<div class="post">
  <div class="header">
    <div class="title">Article Title</div>
    <div class="date">January 1, 2023</div>
  </div>
  <div class="content">
    <div>Article content goes here...</div>
  </div>
</div>
```

#### Accessibility Requirements
```html
<!-- Always include alt text for images -->
<img src="team-photo.jpg" alt="Techium team members collaborating in the office">

<!-- Use proper form labels -->
<label for="email">Email Address</label>
<input type="email" id="email" name="email" required>

<!-- Provide ARIA labels for screen readers -->
<nav aria-label="Main navigation">
  <ul>
    <li><a href="#home" aria-current="page">Home</a></li>
    <li><a href="#about">About</a></li>
  </ul>
</nav>
```

### CSS Guidelines

#### Naming Convention (BEM)
```css
/* Block */
.card { }

/* Element */
.card__title { }
.card__content { }
.card__image { }

/* Modifier */
.card--featured { }
.card--large { }
.card__title--bold { }
```

#### CSS Custom Properties
```css
:root {
  /* Use descriptive, consistent naming */
  --color-primary: #d73953;
  --color-text-primary: #090909;
  --font-family-heading: 'Raleway', sans-serif;
  --spacing-small: 0.5rem;
  --spacing-medium: 1rem;
  --spacing-large: 2rem;
}

/* Use variables consistently */
.button {
  background-color: var(--color-primary);
  font-family: var(--font-family-heading);
  padding: var(--spacing-small) var(--spacing-medium);
}
```

#### CSS Organization
```css
/* Component structure */
.component {
  /* 1. Layout properties */
  display: flex;
  position: relative;
  
  /* 2. Box model */
  width: 100%;
  margin: 0;
  padding: var(--spacing-medium);
  
  /* 3. Typography */
  font-family: var(--font-family-base);
  font-size: var(--font-size-medium);
  
  /* 4. Visual properties */
  background-color: var(--color-white);
  border: 1px solid var(--color-border);
  border-radius: var(--border-radius-small);
  
  /* 5. Animations */
  transition: all 0.3s ease;
}
```

### File Organization

```
project/
├── 0x00-html_advanced/
│   ├── *.html                 # Task files (numbered)
│   ├── index.html            # Final complete page
│   ├── about.html            # Additional pages
│   └── README.md             # Project documentation
│
├── 0x02-CSS_advanced/
│   ├── styles/
│   │   ├── *.css            # Task files (numbered)
│   │   └── normalize.css    # CSS reset
│   ├── images/              # Project assets
│   └── README.md            # Project documentation
│
├── README.md                # Main project documentation
├── CONTRIBUTING.md          # This file
└── DOCUMENTATION.md         # Comprehensive guide
```

## 📝 Commit Guidelines

### Commit Message Format

Use the conventional commit format:

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

#### Types
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **test**: Adding missing tests or correcting existing tests
- **chore**: Changes to the build process or auxiliary tools

#### Examples
```bash
# Feature commit
feat(navigation): add mobile hamburger menu

# Bug fix commit
fix(grid): resolve column alignment issue on mobile

# Documentation commit
docs(readme): update installation instructions

# Style commit
style(css): improve button hover animations

# Refactor commit
refactor(html): improve semantic structure of cards
```

### Commit Best Practices

1. **Make atomic commits** - Each commit should represent a single logical change
2. **Write descriptive messages** - Explain what and why, not just how
3. **Use present tense** - "Add feature" not "Added feature"
4. **Keep the first line under 50 characters**
5. **Add detailed explanation in body if needed**

```bash
# Good commit
feat(hero): add call-to-action button with hover effects

Add a prominent CTA button to the hero section that includes:
- Smooth hover animations
- Accessible focus states
- Responsive sizing for mobile devices

Fixes #42

# Bad commit
fix stuff
```

## 🔀 Pull Request Process

### Before Submitting a PR

1. **Update your branch** with the latest changes:
   ```bash
   git checkout main
   git pull upstream main
   git checkout your-feature-branch
   git rebase main
   ```

2. **Test your changes**:
   - Validate HTML with [W3C Validator](https://validator.w3.org/)
   - Validate CSS with [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
   - Test across different browsers
   - Check responsive design on various screen sizes
   - Verify accessibility with screen readers

3. **Run code quality checks**:
   ```bash
   # Check HTML validation
   # Check CSS validation
   # Test accessibility
   # Verify responsive design
   ```

### PR Title and Description

#### Title Format
```
<type>(<scope>): <description>
```

#### Description Template
```markdown
## Description
Brief description of changes made.

## Type of Change
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation update

## How Has This Been Tested?
- [ ] Browser testing (Chrome, Firefox, Safari, Edge)
- [ ] Mobile responsive testing
- [ ] Accessibility testing
- [ ] HTML/CSS validation

## Screenshots (if applicable)
Add screenshots to help reviewers understand the changes.

## Checklist
- [ ] My code follows the project's coding standards
- [ ] I have performed a self-review of my own code
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] My changes generate no new warnings or errors
- [ ] I have tested my changes across multiple browsers
```

### Review Process

1. **Automated checks** will run on your PR
2. **At least one maintainer** will review your code
3. **Address feedback** by making additional commits
4. **Squash commits** if requested before merging

## 🐛 Issue Reporting

### Before Creating an Issue

1. **Search existing issues** to avoid duplicates
2. **Check documentation** for solutions
3. **Verify the issue** in multiple browsers
4. **Prepare a minimal reproduction** case

### Issue Template

```markdown
## Bug Report

**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Desktop (please complete the following information):**
- OS: [e.g. Windows, macOS, Linux]
- Browser [e.g. Chrome, Safari, Firefox]
- Version [e.g. 22]

**Mobile (please complete the following information):**
- Device: [e.g. iPhone12, Samsung Galaxy S21]
- OS: [e.g. iOS 14.1, Android 11]
- Browser [e.g. Safari, Chrome, Samsung Internet]
- Version [e.g. 22]

**Additional context**
Add any other context about the problem here.
```

### Feature Request Template

```markdown
## Feature Request

**Is your feature request related to a problem? Please describe.**
A clear and concise description of what the problem is.

**Describe the solution you'd like**
A clear and concise description of what you want to happen.

**Describe alternatives you've considered**
A clear and concise description of any alternative solutions or features you've considered.

**Additional context**
Add any other context or screenshots about the feature request here.
```

## 📚 Documentation

### Documentation Standards

1. **Keep documentation up to date** with code changes
2. **Use clear, concise language**
3. **Include code examples** where helpful
4. **Add screenshots** for visual components
5. **Follow markdown standards**

### Documentation Types

#### README Files
- Project overview and objectives
- Installation and setup instructions
- Usage examples
- Contributing guidelines
- License information

#### Code Comments
```html
<!-- Main navigation component -->
<nav class="navigation" aria-label="Main navigation">
  <!-- Navigation items container -->
  <ul class="navigation__list">
    <li class="navigation__item">
      <a href="#home" class="navigation__link" aria-current="page">Home</a>
    </li>
  </ul>
</nav>
```

```css
/* 
 * Card Component
 * 
 * A flexible card component that can be used throughout the site.
 * Supports various modifiers for different use cases.
 * 
 * Usage:
 * <div class="card card--featured">
 *   <div class="card__content">...</div>
 * </div>
 */
.card {
  /* Layout */
  display: flex;
  flex-direction: column;
  
  /* Visual styling */
  background-color: var(--color-white);
  border-radius: var(--border-radius-medium);
  box-shadow: var(--shadow-card);
}
```

## 🧪 Testing

### Manual Testing Checklist

#### HTML Validation
- [ ] All HTML files pass W3C HTML Validator
- [ ] No syntax errors or warnings
- [ ] Proper semantic structure
- [ ] Valid attributes and values

#### CSS Validation
- [ ] All CSS files pass W3C CSS Validator
- [ ] No syntax errors or warnings
- [ ] Proper vendor prefixes where needed
- [ ] Efficient selector usage

#### Cross-Browser Testing
- [ ] Chrome (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest)
- [ ] Edge (latest)
- [ ] Mobile browsers (iOS Safari, Chrome Mobile)

#### Responsive Design
- [ ] Mobile (320px - 767px)
- [ ] Tablet (768px - 1023px)
- [ ] Desktop (1024px+)
- [ ] Large screens (1200px+)

#### Accessibility Testing
- [ ] Keyboard navigation works properly
- [ ] Screen reader compatibility (NVDA, VoiceOver)
- [ ] Color contrast meets WCAG AA standards
- [ ] Images have appropriate alt text
- [ ] Forms are properly labeled
- [ ] Focus indicators are visible

#### Performance Testing
- [ ] Page load time < 3 seconds
- [ ] CSS file size < 50KB (gzipped)
- [ ] Images are optimized
- [ ] No render-blocking resources

### Testing Tools

#### Validation Tools
- [W3C HTML Validator](https://validator.w3.org/)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [WAVE Web Accessibility Evaluator](https://wave.webaim.org/)

#### Browser Testing
- [BrowserStack](https://www.browserstack.com/) (for cross-browser testing)
- Chrome DevTools (for responsive testing)
- Firefox Developer Tools

#### Performance Tools
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [WebPageTest](https://www.webpagetest.org/)
- [GTmetrix](https://gtmetrix.com/)

## 🎯 Code Review Guidelines

### For Contributors

1. **Self-review your code** before submitting
2. **Test thoroughly** across browsers and devices
3. **Write descriptive commit messages**
4. **Respond promptly** to review feedback
5. **Be open to suggestions** and improvements

### For Reviewers

1. **Be constructive and kind** in feedback
2. **Focus on the code, not the person**
3. **Provide specific suggestions** for improvement
4. **Acknowledge good practices** and clever solutions
5. **Test the changes** when possible

### Review Checklist

#### Code Quality
- [ ] Code follows project coding standards
- [ ] Naming conventions are consistent
- [ ] No commented-out code or debug statements
- [ ] Code is readable and well-organized

#### Functionality
- [ ] Changes work as described
- [ ] No breaking changes to existing functionality
- [ ] Edge cases are handled appropriately
- [ ] Error handling is implemented where needed

#### Performance
- [ ] No performance regressions
- [ ] Efficient CSS selectors
- [ ] Optimized images and assets
- [ ] Minimal impact on page load time

#### Accessibility
- [ ] Keyboard navigation support
- [ ] Screen reader compatibility
- [ ] Color contrast compliance
- [ ] Semantic HTML structure

## 🆘 Getting Help

### Where to Ask Questions

1. **GitHub Issues** - For bugs and feature requests
2. **GitHub Discussions** - For general questions and discussions
3. **Discord/Slack** - For real-time communication (if available)

### How to Ask Good Questions

1. **Be specific** about what you're trying to achieve
2. **Include relevant code** snippets or files
3. **Describe what you've tried** already
4. **Mention your environment** (browser, OS, etc.)
5. **Provide screenshots** if applicable

### Resources

- [ALX Intranet](https://intranet.alxswe.com/) - Official ALX resources
- [MDN Web Docs](https://developer.mozilla.org/) - Web standards documentation
- [CSS Tricks](https://css-tricks.com/) - CSS tips and techniques
- [A11y Project](https://www.a11yproject.com/) - Accessibility resources

## 📄 License

By contributing to this project, you agree that your contributions will be licensed under the same license as the project (Educational use as part of ALX curriculum).

## 🙏 Recognition

Contributors will be recognized in the following ways:

1. **Contributors list** in the main README
2. **Commit history** preserves your contributions
3. **Special mentions** for significant contributions
4. **Learning opportunities** through code review process

---

Thank you for contributing to the ALX Frontend Development projects! Your contributions help make this a valuable learning resource for the entire ALX community. 🚀

*Happy coding, and welcome to the team!* 👨‍💻👩‍💻
