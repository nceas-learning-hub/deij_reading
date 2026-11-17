# DEIJ Reading List - Site Structure Guide

## 📁 Project Layout

```
deij_reading/
├── README.md                           # Project documentation
├── SITE_STRUCTURE.md                   # This file
├── _quarto.yml                         # Quarto configuration
├── styles.scss                         # Custom site styling
│
├── index.qmd                           # Home/About page
├── readings.qmd                        # Readings listing page
│
├── readings/                           # Individual reading articles
│   ├── reading-01-race-representation.qmd
│   ├── reading-02-gender-stem.qmd
│   └── reading-03-decolonizing-knowledge.qmd
│
├── images/                             # Images and media
│   ├── logos/
│   │   └── deij-logo.svg              # Site logo
│   ├── reading-1.png                   # Cover image for reading 1
│   ├── reading-2.png                   # Cover image for reading 2
│   └── reading-3.png                   # Cover image for reading 3
│
└── docs/                               # Generated HTML (created by Quarto render)
    ├── index.html
    ├── readings.html
    └── readings/
        ├── reading-01-*.html
        ├── reading-02-*.html
        └── reading-03-*.html
```

## 🎨 Styling & Design

**Color Palette** (Inspired by NCEAS Learning Hub):
- **Primary Dark Green** (#0C4537) - Navigation background
- **Primary Medium Green** (#167B62) - Secondary elements, links
- **Light Green** (#f3f8f7) - Backgrounds, highlights
- **Purple Accent** (#bc40d4) - Interactive elements, hover states
- **Cream** (#F4F3EE) - Cards and light backgrounds

**Fonts**:
- **Headings**: Figtree (modern, geometric sans-serif)
- **Body**: Nunito (readable, friendly sans-serif)

## 📄 Content Pages

### index.qmd (Home/About)
- Welcome message and site overview
- Key themes of the reading list
- Instructions for browsing and using resources
- Call-to-action for contributions

### readings.qmd (Readings Listing)
- Displays all reading articles in a grid
- Filterable by categories
- Sorted by date (most recent first)
- Includes search functionality

### readings/*.qmd (Individual Articles)
Each reading article includes:
- **Title**: Clear, descriptive title
- **Description**: 1-2 sentence summary
- **Image**: Cover image representing the topic
- **Categories**: 2-3 tags for filtering and discovery
- **Date**: When the reading was added
- **Content sections**:
  - Overview
  - Key themes
  - Discussion prompts
  - Related topics

## 🏗️ Building & Rendering

### Render the entire site:
```bash
cd /Users/caseyohara/github/deij_reading
quarto render
```

### Preview changes (live reload):
```bash
quarto preview
```

### Output location:
- All HTML files are generated in the `docs/` folder
- This folder is committed to GitHub and serves the live site

## ➕ Adding New Readings

1. **Create a new .qmd file** in `readings/`
   - Use naming convention: `reading-NN-topic-slug.qmd`
   - Replace NN with sequential number

2. **Include YAML frontmatter**:
   ```yaml
   ---
   title: "Your Reading Title"
   description: "1-2 sentence summary"
   author: "Your Name or DEIJ Reading List"
   date: 2026-11-17
   categories:
     - Topic Category 1
     - Topic Category 2
   image: ../images/your-image.png
   ---
   ```

3. **Add content**:
   - Overview section
   - Key themes (bulleted)
   - Discussion prompts (numbered)
   - Related topics

4. **Add an image**:
   - Create a 6x4 aspect ratio image (e.g., 600x400 or 1200x800)
   - Save to `images/` folder
   - Reference in YAML frontmatter

5. **Render**:
   ```bash
   quarto render
   ```

## 🏷️ Available Categories

Current reading categories used:
- Race & Ethnicity
- Gender & Sexuality
- Representation
- STEM Education
- Workplace Culture
- Indigenous Knowledge Systems
- Environmental Science
- Decolonization
- Accessibility
- General/Interdisciplinary

Feel free to add new categories as needed!

## 📱 Responsive Design

The site is fully responsive and works on:
- Desktop browsers
- Tablets
- Mobile phones

The grid layout automatically adjusts for smaller screens.

## 🔗 Navigation

**Navbar links** (defined in _quarto.yml):
- Home
- Readings (listing page)
- About (submenu)
- GitHub (external link)

**Site footer**:
- Copyright notice
- Built with Quarto

## 🎯 Key Features

✅ Responsive grid layout for reading cards  
✅ Filterable by category tags  
✅ Searchable content  
✅ Modern, accessible color scheme  
✅ Clean typography with Figtree + Nunito  
✅ Easy to extend with new readings  
✅ Built-in SEO optimization  
✅ Static site (no backend required)  

## 📚 Tips for Contributors

- Keep descriptions concise and engaging
- Use discussion prompts to encourage reflection
- Include 3-5 key themes per reading
- Link related readings when relevant
- Use meaningful image alt-text for accessibility
- Keep reading dates current

---

**Last Updated**: November 2026
**Built with**: Quarto + Custom SCSS
