# Quick Setup Guide for Breiss Lab Website

## Welcome! 🎉

Your lab website is ready to go! Follow these simple steps to get it live on the internet.

## Step 1: Enable GitHub Pages (Required - One Time Only)

1. **Go to your repository:** https://github.com/cbreiss/breisslab
2. **Click on "Settings"** (top right, next to the gear icon)
3. **In the left sidebar, click "Pages"**
4. **Under "Source", select:**
   - Source: `GitHub Actions` (from the dropdown)
5. **Done!** Your site will be available at: `https://cbreiss.github.io/breisslab/`

> **Note:** It takes 2-3 minutes after the first commit for your site to go live.

---

## Step 2: Customize Your Site Content

Now let's personalize your website with your lab's information.

### Update Site Title and Contact Info

1. Go to your repository: https://github.com/cbreiss/breisslab
2. Click on `_config.yml`
3. Click the pencil icon (✏️) to edit
4. Update these fields:
   ```yaml
   title: "Your Lab Name"
   email: youremail@university.edu
   description: >-
     Your lab's description goes here
   ```
5. Update the author information:
   ```yaml
   author:
     name: "Your Name"
     bio: "Your title"
     location: "Your University"
     email: "your@email.edu"
   ```
6. Scroll down and click **"Commit changes"**
7. Wait 2-3 minutes and refresh your website!

### Update Your Pages

Edit these files to add your content:

| Page | File to Edit | What to Add |
|------|-------------|-------------|
| **Home** | `index.md` | Welcome message, research highlights |
| **Research** | `_pages/research.md` | Your research areas and projects |
| **People** | `_pages/people.md` | Team member bios and photos |
| **Publications** | `_pages/publications.md` | Your papers and citations |
| **Contact** | `_pages/contact.md` | Contact information and address |

**How to edit:**
1. Click on the file name
2. Click the pencil icon (✏️)
3. Make your changes
4. Click "Commit changes"

---

## Step 3: Add Your First News Post

1. Go to the `_posts` folder
2. Click **"Add file"** → **"Create new file"**
3. Name it: `2024-02-15-my-first-post.md` (use today's date)
4. Copy and paste this template:

```markdown
---
title: "Welcome to Our Lab Website!"
date: 2024-02-15
categories:
  - News
---

We're excited to announce the launch of our new lab website!

Visit us regularly for updates on our research, publications, and team news.
```

5. Click **"Commit new file"**

---

## Step 4: Upload Photos

### Add Team Photos

1. Go to `assets/images/` folder
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop your photos
4. Click **"Commit changes"**
5. Note the exact file name (e.g., `john-doe.jpg`)
6. Update `_pages/people.md` to reference the photo path:
   ```markdown
   ![Photo](/breisslab/assets/images/john-doe.jpg)
   ```

> **Tip:** For profile photos, use square images (400x400 pixels works well)

---

## Need More Help?

📚 **For detailed instructions**, see:
- [README.md](README.md) - Complete documentation
- [CONTENT_GUIDE.md](CONTENT_GUIDE.md) - Content templates and examples

🆘 **Common Issues:**
- **Changes not showing?** Wait 2-3 minutes and hard refresh (Ctrl+F5 / Cmd+Shift+R)
- **Page looks broken?** Check that the `---` lines at the top of files weren't deleted
- **Image not loading?** Make sure the file name matches exactly (case-sensitive!)

---

## Checklist for Launch

Use this to prepare your site for public launch:

- [ ] Enable GitHub Pages in Settings
- [ ] Update site title and description in `_config.yml`
- [ ] Update author/PI information in `_config.yml`
- [ ] Edit home page (`index.md`) with your content
- [ ] Fill in research areas (`_pages/research.md`)
- [ ] Add team member profiles (`_pages/people.md`)
- [ ] Add publications (`_pages/publications.md`)
- [ ] Update contact information (`_pages/contact.md`)
- [ ] Upload team photos to `assets/images/`
- [ ] Create your first news post
- [ ] Test all pages on the live site
- [ ] Share your new website URL! 🎊

---

## What's Next?

After your site is live, you can:

✅ **Regular Updates:**
- Add news posts when papers are published
- Update people page when team members join/leave
- Add new publications to publications page

✅ **Advanced Customization:**
- Change the color scheme (see README.md)
- Add custom pages
- Modify the navigation menu

✅ **Maintenance:**
- Update content regularly
- Keep publications list current
- Respond to inquiries via the contact page

---

## Your Website URL

Once GitHub Pages is enabled, your site will be at:

🌐 **https://cbreiss.github.io/breisslab/**

Share this URL with:
- Your department
- Funding agencies
- Potential students and postdocs
- Collaborators

---

**Congratulations on your new lab website! 🚀**

If you have questions, refer to the detailed guides in README.md and CONTENT_GUIDE.md, or open an issue on GitHub for help.
