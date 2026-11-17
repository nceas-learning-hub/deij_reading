# DEIJ Reading List

A curated collection of resources on diversity, equity, inclusion, and justice (DEIJ) in science, academia, and professional spaces.

## About

This reading list is an effort by the NCEAS DEIJ team to explore ideas of diversity, equity, inclusion, and justice in our conservation science.  A member suggests a reading and leads a discussion on the topic.  The pages here include a link ot the reading, and some reflections on how the reading influenced our thoughts and actions.

## Site Structure

```
deij_reading/
├── _quarto.yml                         # Quarto configuration
├── styles.scss                         # Custom site styling
├── index.qmd                           # Home/About page
├── readings.qmd                        # Readings listing page
├── readings/                           # Individual reading articles
│   ├── yyyy-mm-dd_reading_title_1.qmd
│   ├── yyyy-mm-dd_reading_title_2.qmd
│   └── yyyy-mm-dd_reading_title_3.qmd
│   └── images/                         # Images and media
│       ├── reading1_pic.png            # Cover image for reading 1
│       ├── reading2_photo.jpg          # Cover image for reading 2
│       └── image_reading3.png          # Cover image for reading 3
├── images/                             # Images and media
│   ├── nceas-logo.svg                  # Site logo in banner
│   └── other_image_for_pages.png       # image to go on one of the pages
└── docs/                               # Generated HTML (created by Quarto render)
    ├── <built with quarto render>
```

## Styling

Update in styles.scss

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

3. Add content from Nick's template
4. Run `quarto render` to update the site

## Contributing

Suggestions and contributions are welcome! To suggest a reading or contribute content:

- Open an issue with your suggestion
- Include the reading title, link, and why you think it fits the collection

## License

what license should we use?

## Contact

point of contact?