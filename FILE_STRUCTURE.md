# Website File Structure Explained

This document explains what each file and folder does in your website.

## 📂 Essential Files (Don't Delete!)

### `_config.yml` ⚙️
**What it is:** Main configuration file for your entire website  
**What it controls:**
- Site title and description
- Your name and contact info
- Navigation menu behavior
- Theme settings and colors

**When to edit:** 
- When setting up the site for the first time
- When changing site-wide settings
- Rarely after initial setup

---

### `index.md` 🏠
**What it is:** Your home page  
**What visitors see:** First page when they visit your website  
**When to edit:** 
- Update welcome message
- Add new research highlights
- Change featured content

---

## 📂 Page Folders

### `_pages/` folder
Contains all main pages of your website.

**Files inside:**
- `research.md` - Research page
- `people.md` - Team members page
- `publications.md` - Publications list
- `contact.md` - Contact information

**When to edit:** Whenever you need to update the content on these pages

---

### `_posts/` folder 📰
Contains blog posts and news items.

**File naming:** Must be named `YYYY-MM-DD-title.md`
- Example: `2024-02-15-new-publication.md`
- Example: `2024-03-10-conference-announcement.md`

**When to edit:** 
- Add new posts when you have lab news
- Papers published
- Grants received
- New team members
- Conference presentations

**Note:** Posts automatically appear on your home page (3 most recent)

---

### `_data/` folder
Contains structured data files.

**Files inside:**
- `navigation.yml` - Top menu configuration

**When to edit:** 
- Adding new pages to the top menu
- Reordering menu items
- Rarely needed after initial setup

---

## 📂 Asset Folders

### `assets/images/` folder 🖼️
**What it stores:** All photos and images  
**Recommended subfolders:**
- `people/` - Team member photos
- `research/` - Research-related images
- General images in main folder

**Supported formats:** JPG, PNG, GIF
**When to add files:** 
- Adding team member photos
- Adding research images
- Updating header images

---

### `assets/pdfs/` folder 📄
**What it stores:** PDF files  
**Common files:**
- Published papers
- CVs and resumes
- Posters
- Presentations

**When to add files:**
- Uploading publication PDFs
- Adding CV
- Sharing research materials

---

## 📂 Configuration Files

### `.gitignore`
**What it is:** Tells GitHub which files to ignore  
**Purpose:** Prevents build files and temporary files from being uploaded  
**When to edit:** Rarely - only if you know what you're doing

---

### `Gemfile`
**What it is:** Lists Ruby dependencies needed to run Jekyll  
**Purpose:** Ensures correct versions of software are used  
**When to edit:** Very rarely - only to update Jekyll version

---

### `.github/workflows/pages.yml`
**What it is:** Automatic deployment configuration  
**Purpose:** Tells GitHub how to build and publish your website  
**When to edit:** Never - it's already configured correctly

---

## 📂 Documentation Files

### `README.md` 📖
**What it is:** Complete documentation for the website  
**Who it's for:** You! Reference guide for managing the site  
**When to read:** When you need help with anything

---

### `CONTENT_GUIDE.md` 📝
**What it is:** Templates and examples for common updates  
**Who it's for:** Reference when adding content  
**When to read:** 
- Adding news posts
- Adding team members
- Adding publications
- Learning Markdown formatting

---

### `SETUP.md` 🚀
**What it is:** Quick start guide for first-time setup  
**Who it's for:** Getting the site live for the first time  
**When to read:** Right now! Follow it step by step.

---

## 📂 Generated Folders (Auto-Created)

### `_site/` folder (local only)
**What it is:** Built website files  
**Created when:** Running `bundle exec jekyll build`  
**Important:** This folder is NOT uploaded to GitHub (it's in `.gitignore`)

---

### `Gemfile.lock` (auto-generated)
**What it is:** Locked versions of dependencies  
**Created when:** Running `bundle install`  
**Important:** This file is NOT uploaded to GitHub (it's in `.gitignore`)

---

## Quick Reference: What to Edit When

| I want to... | Edit this file... |
|--------------|-------------------|
| Change site title | `_config.yml` |
| Change my name/email | `_config.yml` |
| Update home page | `index.md` |
| Add research info | `_pages/research.md` |
| Add team member | `_pages/people.md` |
| Add publication | `_pages/publications.md` |
| Update contact info | `_pages/contact.md` |
| Post lab news | Create new file in `_posts/` |
| Add photo | Upload to `assets/images/` |
| Add PDF | Upload to `assets/pdfs/` |
| Change menu | `_data/navigation.yml` |

---

## Visual Structure

```
breisslab/
│
├── 📄 _config.yml          ← Site settings
├── 📄 index.md             ← Home page
│
├── 📁 _pages/              ← Main pages
│   ├── research.md
│   ├── people.md
│   ├── publications.md
│   └── contact.md
│
├── 📁 _posts/              ← Blog posts/news
│   └── YYYY-MM-DD-title.md
│
├── 📁 _data/               ← Site data
│   └── navigation.yml
│
├── 📁 assets/              ← Media files
│   ├── images/
│   │   ├── people/
│   │   └── *.jpg, *.png
│   └── pdfs/
│       └── *.pdf
│
├── 📁 .github/             ← GitHub config
│   └── workflows/
│       └── pages.yml       ← Auto-deployment
│
└── 📚 Documentation
    ├── README.md
    ├── SETUP.md
    ├── CONTENT_GUIDE.md
    └── FILE_STRUCTURE.md   ← You are here!
```

---

## Safety Tips 🛡️

✅ **Safe to edit:**
- Any `.md` file (Markdown content)
- Files in `_data/`
- Adding files to `assets/`

⚠️ **Edit carefully:**
- `_config.yml` (follow the format exactly)
- `.github/workflows/pages.yml` (only if you know YAML)

❌ **Don't delete:**
- `.gitignore`
- `Gemfile`
- `.github/` folder
- Any file starting with underscore (`_`)

---

## Getting Help

If you're not sure which file to edit:
1. Check [CONTENT_GUIDE.md](CONTENT_GUIDE.md) for examples
2. Check [README.md](README.md) for detailed instructions
3. Look at existing files for reference
4. When in doubt, ask before making big changes!

---

**Remember:** GitHub saves every version, so you can always undo changes if something goes wrong! 😊
