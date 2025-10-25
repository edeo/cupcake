# Cupcake Decider

An interactive web application that helps users discover their perfect cupcake through a guided decision tree. Users answer a series of questions about their preferences, and the app recommends a cupcake that matches their taste.

## What is This?

Cupcake Decider is a fun, interactive decision-making tool built as a static website. It guides users through various choices about cupcake flavors, styles, and characteristics to help them decide what kind of cupcake they want.

The application uses a branching question flow where each choice leads to a new set of options, eventually arriving at a cupcake recommendation.

## Features

- **Interactive Decision Tree**: Navigate through questions about flavor preferences
- **Clean Bootstrap UI**: Responsive design that works on all devices
- **Multiple Decision Paths**: Covers various cupcake styles including:
  - Classic flavors vs. unique/adventurous options
  - Chocolate base vs. vanilla base variations
  - Regional comfort food inspired cupcakes (Southern, Tex-Mex, Asian, Midwest, etc.)
- **Easy Navigation**: Simple link-based navigation with a fixed navbar

## Technology Stack

- **HTML5**: Structure and content
- **Bootstrap 3.3.5**: Responsive framework and styling
- **jQuery 1.11.3**: JavaScript functionality
- **Font Awesome**: Icons
- **Highlight.js**: Code syntax highlighting
- **Generated with**: R Markdown/Pandoc (based on metadata)

## Project Structure

```
cupcake/
├── index.html          # Entry point - "What kind" of cupcake
├── about.html          # About page with session information
├── cupcake.html        # Cupcake areas/categories page
├── a*.html             # Decision tree pages (aa.html, aaa.html, aab.html, etc.)
├── style.css           # Custom styles
├── footer.html         # Footer component
├── site_libs/          # Third-party libraries
│   ├── bootstrap-3.3.5/
│   ├── font-awesome-4.5.0/
│   ├── font-awesome-5.1.0/
│   ├── highlightjs-9.12.0/
│   ├── jquery-1.11.3/
│   └── navigation-1.1/
└── README.md           # This file
```

## How to Use

### Viewing the Site Locally

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd cupcake
   ```

2. **Open in a browser**:
   Simply open `index.html` in your web browser:
   ```bash
   # On macOS
   open index.html

   # On Linux
   xdg-open index.html

   # On Windows
   start index.html
   ```

   Or use a local web server:
   ```bash
   # Python 3
   python -m http.server 8000

   # Python 2
   python -m SimpleHTTPServer 8000

   # Node.js (with http-server installed)
   npx http-server
   ```

3. **Navigate the decision tree**:
   - Start at the home page
   - Click on choices that match your preferences
   - Follow the path to discover your ideal cupcake

### Deploying to GitHub Pages

This site is perfect for GitHub Pages:

1. Push the repository to GitHub
2. Go to repository Settings > Pages
3. Select the branch (usually `main` or `master`)
4. The site will be published at `https://<username>.github.io/<repository-name>/`

## Decision Flow Example

```
index.html (What kind?)
├── aa.html (Upgraded classic flavor)
│   ├── aaa.html (Chocolate base)
│   ├── aab.html (Vanilla base)
│   └── aac.html (Both)
└── ab.html (Unique/adventurous)
    ├── aba.html
    ├── abb.html
    └── abc.html
```

## Customization

### Adding New Decision Paths

To add new cupcake options:

1. Create a new HTML file following the existing template
2. Add links to/from existing pages in the decision tree
3. Ensure the navbar and styling are consistent
4. Test all navigation paths

### Modifying Styles

- Edit `style.css` for custom styles
- Modify Bootstrap theme in `site_libs/bootstrap-3.3.5/css/`
- Update navbar in individual HTML files for global navigation changes

## Development

This site was generated using R Markdown, as evidenced by the session information in `about.html`. To modify the source:

1. Edit the R Markdown (.Rmd) files (if available)
2. Knit/render to generate updated HTML files
3. Test changes in a browser

## Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Internet Explorer 9+ (with shims included)
- Mobile browsers (responsive design)

## License

[Add your license information here]

## Contributing

[Add contribution guidelines here]

## Credits

- Built with Bootstrap and R Markdown
- Icons by Font Awesome
- Syntax highlighting by Highlight.js

## About

This interactive cupcake decision tool makes choosing your next cupcake fun and easy. Whether you're looking for a classic flavor with a twist or something completely adventurous, the Cupcake Decider has you covered!
