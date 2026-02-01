# Image Placeholder

This directory should contain images for your website.

## Recommended Structure

```
assets/images/
├── header-image.jpg          # Header image for home page
├── bio-photo.jpg             # PI profile photo
├── people/                   # Team member photos
│   ├── pi-photo.jpg
│   ├── postdoc1.jpg
│   └── student1.jpg
└── research/                 # Research-related images
    └── project1.jpg
```

## Image Guidelines

- **File formats:** Use JPG for photos, PNG for graphics with transparency
- **File sizes:** Optimize images before uploading (aim for < 500KB per image)
- **Dimensions:** 
  - Profile photos: 400x400px (square)
  - Header images: 1920x600px (landscape)
  - Research images: 800x600px or similar
- **Naming:** Use descriptive, lowercase names with hyphens (e.g., `lab-equipment.jpg`)

## Free Stock Photos

If you need placeholder images while setting up:
- [Unsplash](https://unsplash.com/) - Free high-quality photos
- [Pexels](https://pexels.com/) - Free stock photos
- [Pixabay](https://pixabay.com/) - Free images

## How to Add Images

1. Upload image files to this directory via GitHub web interface
2. Reference them in your markdown files using:
   ```markdown
   ![Description](/breisslab/assets/images/filename.jpg)
   ```

Remember to include alt text (the "Description" part) for accessibility!
