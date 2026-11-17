# DEIJ Reading List

A curated collection of resources on diversity, equity, inclusion, and justice (DEIJ) in science, academia, and professional spaces.

## About

This reading list brings together articles, books, reports, and other resources focused on creating more inclusive and equitable scientific communities. Each reading includes:

- A brief summary of key themes
- Relevant category tags for browsing
- Discussion prompts for deeper engagement
- Links to original materials

## Site Structure

```
deij_reading/
├── index.qmd           # Home/about page
├── readings.qmd        # Readings listing page
├── readings/           # Individual reading articles
│   ├── reading-01-*.qmd
│   ├── reading-02-*.qmd
│   └── reading-03-*.qmd
├── images/             # Images for readings and site
│   ├── logos/          # Logo files
│   └── reading-*.png   # Reading cover images
├── styles.scss         # Custom site styling
└── _quarto.yml         # Quarto configuration
```

## Styling

This site uses a custom color palette inspired by the NCEAS Learning Hub theme:

- **Primary Green**: #167B62 (medium green)
- **Dark Green**: #0C4537 (navbar/header)
- **Purple Accent**: #bc40d4 (links and highlights)
- **Light Background**: #F4F3EE (cream)

Fonts:
- **Headings**: Figtree (modern, geometric)
- **Body text**: Nunito (readable, friendly)

## Building the Site

To build the site locally:

```bash
quarto render
```

To preview changes:

```bash
quarto preview
```

## Adding New Readings

To add a new reading:

1. Create a new `.qmd` file in the `readings/` folder
2. Include YAML front matter with:
   - `title`: Reading title
   - `description`: Brief description (1-2 sentences)
   - `author`: Author/contributor name
   - `date`: Publication/added date
   - `categories`: Topic categories (use existing ones or add new)
   - `image`: Path to cover image

3. Add content including discussion prompts
4. Run `quarto render` to update the site

## Contributing

Suggestions and contributions are welcome! To suggest a reading or contribute content:

- Open an issue with your suggestion
- Include the reading title, link, and why you think it fits the collection
- Help us grow this resource!

## License

[Specify your license here - e.g., CC-BY-4.0]

## Contact

[Your contact information here]

---

**Last updated**: November 2026
**Built with**: [Quarto](https://quarto.org/)
