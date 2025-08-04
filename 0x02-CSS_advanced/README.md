# 0x02. CSS Advanced

![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Design-green)
![Modern CSS](https://img.shields.io/badge/Modern-CSS-blue)

## 📖 Description

This project focuses on **advanced CSS concepts** and modern styling techniques to transform the HTML structure from `0x00-html_advanced` into a fully styled, responsive, and interactive **Techium Digital Agency** website. The project emphasizes CSS custom properties, advanced selectors, animations, and responsive design.

## 🎯 Learning Objectives

By the end of this project, you should be able to explain:

- **CSS Fundamentals**:
  - Advanced CSS selectors and specificity
  - CSS custom properties (variables)
  - CSS inheritance and cascade

- **Modern CSS Features**:
  - Flexbox and CSS Grid layouts
  - CSS animations and transitions
  - Responsive design principles
  - CSS methodologies (BEM, OOCSS)

- **Design Systems**:
  - Creating consistent design tokens
  - Building reusable components
  - Maintaining scalable CSS architecture

- **Performance & Optimization**:
  - CSS optimization techniques
  - Cross-browser compatibility
  - Progressive enhancement

## 🗂️ Project Structure

```
0x02-CSS_advanced/
├── README.md                    # This documentation
├── styles/                     # CSS stylesheets directory
│   ├── 1-style.css             # Smooth scrolling
│   ├── 2-style.css             # Color values and variables
│   ├── 3-style.css             # CSS custom properties
│   ├── 4-style.css             # Font family variables
│   ├── 5-style.css             # Font size variables
│   ├── 6-style.css             # Font weight variables
│   ├── 7-style.css             # Google Fonts integration
│   ├── 8-style.css             # Line height variables
│   ├── 9-style.css             # Link styling
│   ├── 10-style.css            # Section centering
│   ├── 11-style.css            # Section tagline styling
│   ├── 12-style.css            # Section title styling
│   ├── 13-style.css            # Pseudo-classes
│   ├── 14-style.css            # CSS normalization
│   ├── 15-style.css            # Universal box-sizing
│   ├── 16-style.css            # Container styling
│   ├── 17-style.css            # Section padding
│   ├── 18-style.css            # Navigation styling
│   ├── 19-style.css            # Grid system
│   ├── 20-style.css            # Grid cleanup
│   ├── 21-style.css            # Column selectors
│   ├── 22-style.css            # Dark theme
│   ├── 23-style.css            # Footer styling
│   ├── 24-style.css            # Service cards
│   ├── 25-style.css            # Button styling
│   ├── 26-style.css            # Testimonial styling
│   ├── 27-style.css            # Hero section
│   ├── 28-style.css            # Header navigation
│   ├── 29-style.css            # Navigation effects
│   ├── 30-style.css            # Work portfolio styling
│   ├── 31-style.css            # Quote decorations
│   └── 32-style.css            # Transitions and animations
└── images/                     # Project assets
    ├── pic-about-01.jpg        # About section image
    ├── pic-article-01.jpg      # Article images
    ├── pic-article-02.jpg
    ├── pic-article-03.jpg
    ├── pic-person-01.jpg       # Team member photos
    ├── pic-person-02.jpg
    ├── pic-person-03.jpg
    ├── pic-work-01.jpg         # Portfolio images
    ├── pic-work-02.jpg
    └── pic-work-03.jpg
```

## 🎨 Design System

### 🎭 Color Palette
```css
:root {
  --color-primary: #d73953;      /* Brand Pink */
  --color-black: #090909;        /* Near Black */
  --color-white: #ffffff;        /* Pure White */
  --color-light-grey: #f3f3f3;   /* Light Grey */
  --color-dark-grey: #353535;    /* Dark Grey */
  --text-color: var(--color-black);
}
```

### 🔤 Typography System
```css
:root {
  /* Font Families */
  --font-family-base: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  --font-family-title: 'Raleway', 'Helvetica Neue', Helvetica, Arial, sans-serif;

  /* Font Sizes (Responsive Scale) */
  --font-size-small: 1.2rem;     /* 12px */
  --font-size-medium: 1.6rem;    /* 16px */
  --font-size-large: 1.8rem;     /* 18px */
  --font-size-x-large: 2.3rem;   /* 23px */
  --font-size-xx-large: 4.8rem;  /* 48px */

  /* Font Weights */
  --font-weight-regular: 400;
  --font-weight-bold: 700;

  /* Line Heights */
  --line-height-small: 1.2;
  --line-height-base: 1.5;
  --line-height-big: 1.8;
}
```

### 📐 Spacing System
```css
:root {
  /* Section Spacing */
  --section-padding: 5rem 0;
  --section-header-padding: 0 0 3rem;
  --section-body-padding: 0 0 3rem;
  --section-footer-padding: 3rem 0 0;

  /* Component Spacing */
  --container-max-width: 960px;
  --button-padding: 1.5rem 3rem;
  --nav-item-margin: 3rem 0 0 0;
}
```

## 📋 Task Progression

| Task | File | Focus | Key Concepts |
|------|------|-------|--------------|
| 1 | `1-style.css` | Smooth Scrolling | `scroll-behavior: smooth` |
| 2 | `2-style.css` | Color Values | Hex colors, color theory |
| 3 | `3-style.css` | CSS Variables | Custom properties, `:root` |
| 4 | `4-style.css` | Font Variables | Typography system |
| 5 | `5-style.css` | Font Sizes | Responsive typography |
| 6 | `6-style.css` | Font Weights | Typography hierarchy |
| 7 | `7-style.css` | Google Fonts | Web font integration |
| 8 | `8-style.css` | Line Heights | Vertical rhythm |
| 9 | `9-style.css` | Link Styling | Text decoration, states |
| 10 | `10-style.css` | Text Alignment | Centering techniques |
| 11 | `11-style.css` | Text Transform | Typography effects |
| 12 | `12-style.css` | Section Titles | Heading styles |
| 13 | `13-style.css` | Pseudo-classes | `:hover`, `:active`, `:visited` |
| 14 | `14-style.css` | Normalize CSS | Browser reset |
| 15 | `15-style.css` | Box Sizing | `box-sizing: border-box` |
| 16 | `16-style.css` | Container | Layout containers |
| 17 | `17-style.css` | Padding | Spacing system |
| 18 | `18-style.css` | Navigation | Menu styling |
| 19 | `19-style.css` | Grid System | Layout foundations |
| 20 | `20-style.css` | Clearfix | Float clearing |
| 21 | `21-style.css` | Selectors | Attribute selectors |
| 22 | `22-style.css` | Dark Theme | Theme switching |
| 23 | `23-style.css` | Footer | Footer styling |
| 24 | `24-style.css` | Service Cards | Card components |
| 25 | `25-style.css` | Buttons | Interactive elements |
| 26 | `26-style.css` | Testimonials | User content |
| 27 | `27-style.css` | Hero Section | Landing area |
| 28 | `28-style.css` | Header | Site header |
| 29 | `29-style.css` | Nav Effects | Hover animations |
| 30 | `30-style.css` | Portfolio | Image galleries |
| 31 | `31-style.css` | Decorations | CSS art |
| 32 | `32-style.css` | Transitions | Smooth animations |

## 🛠️ Technologies & Techniques

### CSS Features Used
- **CSS Custom Properties**: For maintainable theming
- **Advanced Selectors**: Attribute, pseudo-class, combinators
- **Flexbox**: For flexible layouts
- **CSS Grid**: For complex layouts
- **Animations**: CSS transitions and keyframes
- **Responsive Design**: Mobile-first approach

### Methodologies Applied
- **BEM**: Block, Element, Modifier naming
- **OOCSS**: Object-Oriented CSS principles
- **Mobile-First**: Progressive enhancement
- **Component-Based**: Reusable UI components

### Browser Support
- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ⚠️ IE11 (partial support)

## 🚀 Getting Started

### Prerequisites
- Modern web browser
- Text editor with CSS support
- Basic understanding of HTML/CSS

### Installation
```bash
# Clone the repository
git clone https://github.com/salmaneben/alx-frontend.git
cd alx-frontend/0x02-CSS_advanced

# Start a local server
python -m http.server 8000
# Visit http://localhost:8000
```

### Development Workflow
1. **Edit CSS files** in the `styles/` directory
2. **Link stylesheets** to HTML files
3. **Test in browsers** for compatibility
4. **Validate CSS** using W3C validator
5. **Optimize performance** before deployment

## 🎯 Key Features Implemented

### 1. **Responsive Grid System**
```css
.row {
  margin: 0;
  padding: 0;
  list-style: none;
}

.row::after {
  content: "";
  display: table;
  clear: both;
}

[class^="col-"] {
  float: left;
  padding: 0.5rem;
}

.col-1-3 { width: 33.33%; }
.col-1-2 { width: 50%; }
```

### 2. **Interactive Navigation**
```css
.nav .nav-link::before {
  content: '';
  position: absolute;
  background-color: var(--color-primary);
  width: 0;
  height: 0.2rem;
  transition: width 0.3s ease;
}

.nav .nav-item:hover .nav-link::before {
  width: 100%;
}
```

### 3. **Card Components**
```css
.card-services a {
  display: block;
  padding: 2rem;
  background-color: var(--color-light-grey);
  transition: all 0.3s ease;
}

.card-services a:hover {
  color: var(--color-white);
  background-color: var(--color-primary);
  transform: scale(1.05);
}
```

### 4. **Dark Theme Support**
```css
[data-section-theme="dark"] {
  --text-color: var(--color-white);
  --section-title-color: var(--color-white);
  background-color: var(--color-black);
}
```

## 📱 Responsive Design

### Breakpoint System
```css
/* Mobile First Approach */
/* Base styles: 320px and up */

/* Tablet: 768px and up */
@media (min-width: 768px) {
  .container { max-width: 768px; }
}

/* Desktop: 1024px and up */
@media (min-width: 1024px) {
  .container { max-width: 960px; }
}

/* Large Desktop: 1200px and up */
@media (min-width: 1200px) {
  .container { max-width: 1140px; }
}
```

### Responsive Typography
```css
html {
  font-size: 62.5%; /* 1rem = 10px */
}

/* Responsive scaling */
@media (max-width: 480px) {
  html { font-size: 57%; }
}

@media (min-width: 1200px) {
  html { font-size: 65%; }
}
```

## 🎨 Advanced CSS Techniques

### 1. **CSS Custom Properties (Variables)**
```css
:root {
  --primary-color: #d73953;
  --transition-duration: 0.3s;
  --border-radius: 0.5rem;
}

/* Usage with fallbacks */
.button {
  background-color: var(--primary-color, #d73953);
  transition: all var(--transition-duration, 0.3s) ease;
}
```

### 2. **Advanced Selectors**
```css
/* Attribute selectors */
[class^="col-"] { /* Starts with "col-" */ }
[class*="button"] { /* Contains "button" */ }
[data-theme="dark"] { /* Exact attribute match */ }

/* Combinators */
.nav > .nav-item { /* Direct children */ }
.section + .section { /* Adjacent siblings */ }
.card ~ .card { /* General siblings */ }
```

### 3. **Pseudo-elements for Decorations**
```css
.card-testimonial .card-quote::before {
  content: '\201C'; /* Left double quotation mark */
  position: absolute;
  font-size: 10rem;
  color: var(--color-light-grey);
  z-index: -1;
}
```

### 4. **Smooth Animations**
```css
:root {
  --transition-duration: 0.3s;
  --transition-timing: cubic-bezier(0.17, 0.67, 0, 1.01);
}

.card-work:hover .card-image img {
  transform: scale(1.2);
  transition: transform var(--transition-duration) var(--transition-timing);
}
```

## 🔧 Performance Optimization

### CSS Optimization
- **Minification**: Remove whitespace and comments
- **Critical CSS**: Inline above-the-fold styles
- **Unused CSS**: Remove unused selectors
- **Efficient Selectors**: Avoid overly specific selectors

### Loading Optimization
```html
<!-- Preload critical fonts -->
<link rel="preload" href="fonts/OpenSans-Regular.woff2" as="font" type="font/woff2" crossorigin>

<!-- Non-blocking CSS -->
<link rel="stylesheet" href="styles/style.css" media="all">
```

## ♿ Accessibility Features

### Focus Management
```css
.button:focus {
  outline: 2px solid var(--color-primary);
  outline-offset: 2px;
}

/* Custom focus indicators */
.nav-link:focus::before {
  background-color: var(--color-primary);
  width: 100%;
}
```

### Color Contrast
- All text meets WCAG AA standards (4.5:1 ratio)
- Interactive elements have sufficient contrast
- Color is not the only means of conveying information

### Reduced Motion
```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

## 📊 Browser Compatibility

### CSS Feature Support
- **Custom Properties**: ✅ All modern browsers
- **Flexbox**: ✅ All modern browsers, IE11 with prefixes
- **Grid**: ✅ All modern browsers, IE11 partial
- **Transitions**: ✅ All browsers

### Fallback Strategies
```css
/* Flexbox fallbacks */
.nav-item {
  display: inline-block; /* Fallback */
  display: flex; /* Modern browsers */
}

/* Custom property fallbacks */
.button {
  background: #d73953; /* Fallback */
  background: var(--color-primary); /* Modern browsers */
}
```

## 🧪 Testing & Validation

### CSS Validation
- All CSS passes [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- No syntax errors or invalid properties
- Vendor prefixes used where necessary

### Cross-browser Testing
- Manual testing in major browsers
- Automated testing with tools like BrowserStack
- Progressive enhancement verification

### Performance Testing
- Lighthouse audits for performance metrics
- CSS file size optimization
- Render-blocking resource identification

## 📚 Resources & References

### CSS Specifications
- [CSS3 Specifications - W3C](https://www.w3.org/Style/CSS/)
- [MDN CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Can I Use](https://caniuse.com/) - Browser compatibility

### Design Resources
- [CSS Tricks](https://css-tricks.com/)
- [Smashing Magazine](https://www.smashingmagazine.com/)
- [A List Apart](https://alistapart.com/)

### Tools & Validators
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [PostCSS](https://postcss.org/) - CSS processing
- [Autoprefixer](https://autoprefixer.github.io/) - Vendor prefixes

## 🎯 Skills Developed

- [x] Advanced CSS selectors and specificity
- [x] CSS custom properties and theming
- [x] Responsive design and mobile-first approach
- [x] CSS animations and transitions
- [x] Cross-browser compatibility
- [x] Performance optimization
- [x] Accessibility implementation
- [x] Modern CSS methodologies

## 🔄 Future Enhancements

### Planned Improvements
- [ ] CSS Grid implementation for complex layouts
- [ ] Advanced animations with `@keyframes`
- [ ] CSS-in-JS integration for dynamic theming
- [ ] PWA features with CSS
- [ ] Dark/light mode toggle functionality

### Advanced Topics
- [ ] CSS Subgrid
- [ ] Container queries
- [ ] CSS Houdini
- [ ] CSS-in-JS patterns

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Test across browsers
4. Validate CSS
5. Submit a pull request

## 👨‍💻 Author

**Salman Eben**
- GitHub: [@salmaneben](https://github.com/salmaneben)
- Project: ALX Software Engineering Program

## 📄 License

This project is part of the ALX Software Engineering curriculum.

---

*Crafting beautiful, accessible, and performant web experiences with modern CSS! 🎨*