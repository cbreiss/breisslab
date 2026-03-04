# Breiss Lab Website

Welcome to the Breiss Lab website repository! This site is built with Jekyll using the Minimal Mistakes theme and is automatically deployed to GitHub Pages.

🌐 **Live Website:** [https://cbreiss.github.io/breisslab/](https://cbreiss.github.io/breisslab/)

---

## 🚀 First Time Setup

**Before you can use the website, you MUST enable GitHub Pages:**

👉 **See [GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md) for detailed setup instructions**

**Quick summary:**
1. Go to your repository Settings
2. Click "Pages" in the left sidebar  
3. Set Source to "GitHub Actions"
4. Your site will be live in 2-3 minutes!

---

## 📋 Quick Start for Beginners

This guide is designed for people who are **not familiar with GitHub or programming**. Follow these simple steps to update your website.

### How to Edit Your Website (Using GitHub Web Interface)

You can update your website directly from your web browser - no coding knowledge required!

#### 1. **Edit a Page**

1. Go to https://github.com/cbreiss/breisslab
2. Click on the folder or file you want to edit:
   - **Home page**: Click `index.md`
   - **Research page**: Click `_pages` folder, then `research.md`
   - **People page**: Click `_pages` folder, then `people.md`
   - **Publications page**: Click `_pages` folder, then `publications.md`
   - **Contact page**: Click `_pages` folder, then `contact.md`
3. Click the pencil icon (✏️) in the top right that says "Edit this file"
4. Make your changes in the text editor
5. Scroll down and click the green "Commit changes" button
6. Wait 2-3 minutes for your changes to appear on the live website!

#### 2. **Add a News Post**

1. Go to the `_posts` folder
2. Click "Add file" → "Create new file"
3. Name your file: `YYYY-MM-DD-title.md` (e.g., `2024-02-15-new-grant.md`)
4. Add content following this template:

```markdown
---
title: "Your Post Title"
date: 2024-02-15
categories:
  - News
tags:
  - research
---

Your news content goes here. You can write in plain text or use markdown formatting.

## Subheadings

- Bullet points
- More points

**Bold text** and *italic text*
```

5. Click "Commit new file"

#### 3. **Add Team Member Photos**

1. Go to the `assets/images` folder
2. Click "Add file" → "Upload files"
3. Drag and drop your photo files
4. Click "Commit changes"
5. Update the `_pages/people.md` file to reference the new photo

#### 4. **Update Site Settings**

To change site-wide settings (site title, your email, social media links):
1. Click on `_config.yml`
2. Click the pencil icon (✏️) to edit
3. Update the information (be careful to keep the same format!)
4. Commit your changes

### Important Notes

- **Changes take 2-3 minutes to appear** on your live website after committing
- **Always use the format** shown in the example files
- **The dashes `---` at the top** of files are important - don't delete them!
- **Test your changes** by viewing the live site after a few minutes

---

## 📁 Website Structure

Here's what each folder and file does:

```
breisslab/
├── _config.yml           # Main site settings (title, description, author info)
├── index.md              # Home page
├── _pages/               # Main website pages
│   ├── research.md       # Research page
│   ├── people.md         # People/team page
│   ├── publications.md   # Publications list
│   └── contact.md        # Contact information
├── _posts/               # Blog posts/news items
│   └── YYYY-MM-DD-title.md
├── _data/
│   └── navigation.yml    # Top menu navigation
├── assets/
│   └── images/           # Photos and images
└── .github/
    └── workflows/        # Automatic deployment settings
```

---

## ✏️ How to Customize Your Site

### Change Site Title and Description

Edit `_config.yml`:

```yaml
title: "Your Lab Name"
description: "Your lab description"
email: youremail@university.edu
```

### Change the Theme Color

Edit `_config.yml` and change:

```yaml
minimal_mistakes_skin: "default"
```

Options: `"air"`, `"aqua"`, `"contrast"`, `"dark"`, `"dirt"`, `"neon"`, `"mint"`, `"plum"`, `"sunrise"`

### Update Principal Investigator Information

Edit the `author:` section in `_config.yml`:

```yaml
author:
  name: "Your Name"
  avatar: "/assets/images/your-photo.jpg"
  bio: "Your title and affiliation"
  location: "Your Location"
  email: "your@email.edu"
```

### Add New Menu Items

Edit `_data/navigation.yml`:

```yaml
main:
  - title: "New Page"
    url: /new-page/
```

Then create a corresponding page in the `_pages/` folder.

---

## 🎓 For Advanced Users

### Running the Site Locally

If you want to preview changes before publishing:

1. **Install Ruby and Bundler** (if not already installed)
2. **Clone this repository:**
   ```bash
   git clone https://github.com/cbreiss/breisslab.git
   cd breisslab
   ```
3. **Install dependencies:**
   ```bash
   bundle install
   ```
4. **Run the local server:**
   ```bash
   bundle exec jekyll serve
   ```
5. **View in browser:** Open http://localhost:4000/breisslab/

### Markdown Formatting Guide

- `# Heading 1` → Large heading
- `## Heading 2` → Smaller heading
- `**bold text**` → **bold text**
- `*italic text*` → *italic text*
- `[link text](url)` → Clickable link
- `![alt text](image-url)` → Image
- `- item` → Bullet point
- `1. item` → Numbered list

---

## 🚀 GitHub Pages Setup

Your site is automatically deployed using GitHub Actions. To ensure everything works:

1. **Go to your repository settings** (Settings tab)
2. **Navigate to "Pages"** (in the left sidebar)
3. **Under "Source"**, select:
   - Source: `GitHub Actions`
4. Your site will be available at: `https://cbreiss.github.io/breisslab/`

---

## 🆘 Getting Help

### Common Issues

**Problem:** Changes aren't showing up on the website
- **Solution:** Wait 2-3 minutes after committing. Check the "Actions" tab to see if the build succeeded.

**Problem:** Website shows an error after editing
- **Solution:** Check that you didn't accidentally delete the `---` lines at the top of files. Revert your last change if needed.

**Problem:** Images aren't displaying
- **Solution:** Make sure image file names match exactly in your markdown files (case-sensitive!)

### Resources

- **Jekyll Documentation:** https://jekyllrb.com/docs/
- **Minimal Mistakes Theme:** https://mmistakes.github.io/minimal-mistakes/
- **Markdown Guide:** https://www.markdownguide.org/basic-syntax/
- **GitHub Pages:** https://docs.github.com/en/pages

---

## 📝 Content Update Checklist

Use this checklist when setting up your site for the first time:

- [ ] Update site title and description in `_config.yml`
- [ ] Update author information in `_config.yml`
- [ ] Replace email addresses throughout the site
- [ ] Update the home page (`index.md`)
- [ ] Fill in research areas (`_pages/research.md`)
- [ ] Add team member profiles (`_pages/people.md`)
- [ ] Add publications (`_pages/publications.md`)
- [ ] Update contact information (`_pages/contact.md`)
- [ ] Upload team photos to `assets/images/`
- [ ] Delete example content and replace with real content
- [ ] Create your first news post in `_posts/`
- [ ] Test all links and pages

---

## 📚 Documentation Files

This repository includes several guides to help you:

- **[GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md)** - ⭐ Detailed GitHub Pages setup with visual guides
- **[GETTING_STARTED.md](GETTING_STARTED.md)** - Overview of what was created and next steps  
- **[SETUP.md](SETUP.md)** - Quick setup checklist
- **[CONTENT_GUIDE.md](CONTENT_GUIDE.md)** - Templates for adding content (news, people, publications)
- **[FILE_STRUCTURE.md](FILE_STRUCTURE.md)** - Explanation of all files and folders

**Start here:** If you haven't enabled GitHub Pages yet, begin with [GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md)!

---

## 📄 License

This website template is based on the Minimal Mistakes Jekyll theme, which is © 2013-2024 Michael Rose and contributors under the MIT License.

---

**Need help?** Check [GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md) for detailed setup instructions, or open an issue on this repository!
