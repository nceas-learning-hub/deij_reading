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
│   ├── yyyy-mm-dd_reading_title_1.qmd
│   ├── yyyy-mm-dd_reading_title_2.qmd
│   └── yyyy-mm-dd_reading_title_3.qmd
│   └── images/                         # Images and media
│       ├── reading1_pic.png            # Cover image for reading 1
│       ├── reading2_photo.jpg          # Cover image for reading 2
│       └── image_reading3.png          # Cover image for reading 3
│
├── images/                             # Images and media
│   ├── nceas-logo.svg                  # Site logo in banner
│   └── other_image_for_pages.png       # image to go on one of the pages
│
└── docs/                               # Generated HTML (created by Quarto render)
    ├── index.html
    ├── readings.html
    └── readings/
        ├── reading-01-*.html
        ├── reading-02-*.html
        └── reading-03-*.html
```

