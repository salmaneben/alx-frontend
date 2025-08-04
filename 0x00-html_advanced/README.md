# 0x00. HTML Advanced

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![Semantic Web](https://img.shields.io/badge/Semantic-Web-orange)
![Accessibility](https://img.shields.io/badge/Accessibility-WCAG-green)

## 📖 Description

This project focuses on mastering **HTML5 semantic elements** and building the structure for a modern, accessible digital agency website called **"Techium"**. The emphasis is on semantic markup, document structure, accessibility, and following web standards without any CSS styling.

## 🎯 Learning Objectives

By the end of this project, you should be able to explain:

- **HTML Fundamentals**:
  - What is HTML and its role in web development
  - How to create an HTML5 page structure
  - The importance of semantic elements

- **Semantic HTML**:
  - What is a markup language and semantic HTML
  - How to use HTML5 semantic elements properly
  - The difference between `<div>` and semantic elements

- **Document Structure**:
  - How to structure a web page with proper hierarchy
  - When and how to use headings (h1-h6)
  - The importance of document outline

- **Accessibility & SEO**:
  - How to make HTML accessible for screen readers
  - The importance of alt attributes and ARIA labels
  - How to optimize HTML for search engines

## 🗂️ Project Structure

```
0x00-html_advanced/
├── README.md                    # This documentation
├── 0-index.html                # Basic HTML structure
├── 1-index.html                # Add head and body
├── 2-index.html                # Meta charset
├── 3-index.html                # Meta viewport
├── 5-index.html                # Meta tags & favicon
├── 6-index.html                # Basic page structure
├── 7-index.html                # Add sections
├── 8-index.html                # Navigation
├── 9-index.html                # Heading hierarchy  
├── 10-index.html               # Add content sections
├── 11-styleguide.html          # Style guide foundation
├── 12-index.html               # Enhance sections
├── 13-styleguide.html          # Styleguide paragraphs
├── 14-index.html               # Div containers
├── 15-index.html               # Structure improvements
├── 16-index.html               # More structure
├── 17-index.html               # Comments and content
├── 18-index.html               # Links and navigation
├── 20-index.html               # Internal links
├── 21-index.html               # Social media links
├── 22-index.html               # Enhanced content
├── 23-index.html               # Service links
├── 24-index.html               # Portfolio links
├── 25-index.html               # Footer links
├── 26-styleguide.html          # Footer in styleguide
├── 27-index.html               # Copyright footer
├── 28-styleguide.html          # Additional styleguide
├── 29-index.html               # Menu navigation
├── 30-styleguide.html          # Styleguide lists
├── 31-index.html               # Contact information
├── 32-styleguide.html          # Tables and code
├── 33-styleguide.html          # Enhanced styleguide
├── 34-styleguide.html          # More styleguide elements
├── 35-index.html               # Image integration
├── 36-index.html               # Portfolio images
├── 38-styleguide.html          # Media elements
├── 39-styleguide.html          # Audio elements
├── index.html                  # Final complete page
├── about.html                  # About page
├── contact.html                # Contact page
├── article.html                # Article page
├── latest_news.html            # News page
└── styleguide.html             # Complete style guide
```

## 🎨 The Techium Project

**Techium** is a fictional digital agency website that showcases:

### 🏗️ Website Structure
- **Header**: Logo, navigation menu
- **Main Content**:
  - Hero section with call-to-action
  - Services showcase
  - Portfolio/Works gallery
  - About us section
  - Latest news/blog
  - Testimonials
  - Contact information
- **Footer**: Social links, legal pages, copyright

### 🎯 Key Features Implemented

1. **Semantic HTML5 Elements**:
   ```html
   <header>    <!-- Site header -->
   <nav>       <!-- Navigation menus -->
   <main>      <!-- Main content area -->
   <section>   <!-- Content sections -->
   <article>   <!-- Standalone content -->
   <aside>     <!-- Sidebar content -->
   <footer>    <!-- Site footer -->
   ```

2. **Proper Meta Tags**:
   ```html
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta name="description" content="Techium is a digital agency">
   ```

3. **Accessibility Features**:
   - Semantic structure for screen readers
   - Proper heading hierarchy (h1-h6)
   - Alt attributes for images
   - Descriptive link text
   - ARIA labels where needed

4. **SEO Optimization**:
   - Proper title tags
   - Meta descriptions
   - Semantic markup
   - Structured content hierarchy

## 📋 Tasks Overview

| Task | File | Description |
|------|------|-------------|
| 0 | `0-index.html` | Create basic HTML5 structure |
| 1 | `1-index.html` | Add head and body sections |
| 2 | `2-index.html` | Add meta charset |
| 3 | `3-index.html` | Add meta viewport |
| 4 | `4-index.html` | Add meta tags |
| 5 | `5-index.html` | Add favicon |
| 6 | `6-index.html` | Add page structure |
| 7 | `7-index.html` | Add sections |
| 8 | `8-index.html` | Add navigation |
| 9 | `9-index.html` | Add headings |
| 10 | `10-index.html` | Add more content |
| ... | ... | ... |
| Final | `index.html` | Complete website |

## 🛠️ Technologies Used

- **HTML5**: Latest HTML standard
- **Semantic Elements**: For meaningful structure
- **Meta Tags**: For SEO and responsive design
- **Accessibility**: WCAG guidelines compliance

## 🚀 Getting Started

### Prerequisites
- Any modern web browser
- Text editor (VS Code, Sublime Text, etc.)

### Running the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/salmaneben/alx-frontend.git
   cd alx-frontend/0x00-html_advanced
   ```

2. **Open in browser**:
   ```bash
   # Double-click any HTML file, or
   # Use a local server
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

3. **View specific tasks**:
   - Open individual HTML files to see progression
   - Compare different versions to understand concepts

## 📖 Key Concepts Learned

### 1. **HTML5 Semantic Elements**
```html
<!-- Instead of generic divs -->
<div class="header">...</div>
<div class="navigation">...</div>
<div class="main-content">...</div>

<!-- Use semantic elements -->
<header>...</header>
<nav>...</nav>
<main>...</main>
```

### 2. **Proper Document Structure**
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
</head>
<body>
    <header>...</header>
    <main>...</main>
    <footer>...</footer>
</body>
</html>
```

### 3. **Accessibility Best Practices**
```html
<!-- Images with alt text -->
<img src="image.jpg" alt="Descriptive text">

<!-- Proper form labels -->
<label for="email">Email Address</label>
<input type="email" id="email" name="email">

<!-- Heading hierarchy -->
<h1>Main Title</h1>
<h2>Section Title</h2>
<h3>Subsection Title</h3>
```

### 4. **SEO Optimization**
```html
<head>
    <title>Homepage - Techium</title>
    <meta name="description" content="Techium is a digital agency">
    <link rel="canonical" href="https://example.com">
</head>
```

## ✅ Validation and Testing

### HTML Validation
- All HTML files pass [W3C HTML Validator](https://validator.w3.org/)
- No syntax errors or warnings
- Proper nesting and structure

### Accessibility Testing
- Screen reader compatibility
- Keyboard navigation support
- Proper contrast ratios (when CSS is added)
- ARIA compliance

### Browser Compatibility
- Chrome/Chromium ✅
- Firefox ✅
- Safari ✅
- Edge ✅

## 📚 Resources

### Official Documentation
- [HTML5 Specification - W3C](https://www.w3.org/TR/html52/)
- [MDN HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [WHATWG HTML Living Standard](https://html.spec.whatwg.org/)

### Accessibility
- [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/WCAG21/quickref/)
- [A11y Project](https://www.a11yproject.com/)
- [WebAIM](https://webaim.org/)

### SEO
- [Google Search Central](https://developers.google.com/search)
- [Schema.org](https://schema.org/)

## 🔍 Advanced Topics Covered

### Semantic HTML Benefits
1. **Accessibility**: Screen readers understand content structure
2. **SEO**: Search engines better index semantic content
3. **Maintainability**: Code is more readable and maintainable
4. **Future-proof**: Semantic markup adapts to new technologies

### Document Outline
- Proper heading hierarchy creates document outline
- Each page should have one h1 element
- Headings should not skip levels
- Sections should be properly nested

### Microdata and Schema
- Structured data for search engines
- Rich snippets in search results
- Better content understanding

## 🎯 Skills Developed

- [x] HTML5 semantic structure
- [x] Document hierarchy and outline
- [x] Accessibility implementation
- [x] SEO-friendly markup
- [x] Cross-browser compatibility
- [x] Web standards compliance
- [x] Progressive enhancement mindset

## 🤝 Contributing

This is an educational project. If you find any issues:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test across browsers
5. Submit a pull request

## 📝 Notes

- **No CSS**: This project focuses purely on HTML structure
- **Progressive Enhancement**: Start with solid HTML foundation
- **Semantic First**: Choose elements based on meaning, not appearance
- **Accessibility**: Consider all users from the beginning

## 👨‍💻 Author

**Salman Eben**
- GitHub: [@salmaneben](https://github.com/salmaneben)
- Project: ALX Software Engineering Program

## 📄 License

This project is part of the ALX Software Engineering curriculum.

---

*Building the web with semantic HTML - one element at a time! 🏗️*