# 📘 Detailed GitHub Pages Setup Guide

## How to Enable GitHub Pages - Step by Step

This guide provides **detailed, visual instructions** for enabling GitHub Pages. Follow each step carefully.

---

## 🎯 Goal

Enable GitHub Pages so your website becomes live at: `https://cbreiss.github.io/breisslab/`

**Time needed:** 5 minutes

---

## 📍 Step-by-Step Instructions

### Step 1: Navigate to Your Repository

1. Open your web browser
2. Go to: **https://github.com/cbreiss/breisslab**
3. You should see the main page of your repository with all the files

---

### Step 2: Open Repository Settings

**Look at the TOP of the page**, you'll see a horizontal menu bar with tabs:

```
< > Code    Issues    Pull requests    Actions    Projects    Wiki    Security    Insights    Settings
```

1. **Click on the "Settings" tab** (it's the LAST item on the right in the menu bar)
   - If you don't see "Settings", you may not have admin access to the repository
   - The owner of the repository needs to do this step

**What you'll see:**
- The page will change to show various settings options
- You'll see a long sidebar on the LEFT side with many options

---

### Step 3: Find the "Pages" Setting

**Look at the LEFT sidebar**. You'll see a list of options:

```
General
Access
    Collaborators
    Moderation
Code and automation
    Branches
    Tags
    Actions
    Webhooks
    Environments
    Codespaces
    Pages          ← CLICK HERE!
    Custom properties
```

1. **Scroll down in the left sidebar** until you see **"Pages"**
   - It's in the "Code and automation" section
   - It's usually between "Environments" and "Custom properties"
   
2. **Click on "Pages"**

**What you'll see:**
- The main area will now show "GitHub Pages" settings
- At the top it says "GitHub Pages"

---

### Step 4: Configure the Source

**In the main area, look for the section titled "Build and deployment"**

You'll see:
```
Source
[Dropdown menu showing current selection]
```

1. **Click on the dropdown menu** under "Source"
   
2. **You'll see two options:**
   - Deploy from a branch
   - GitHub Actions  ← **SELECT THIS ONE**

3. **Click "GitHub Actions"**

**What happens:**
- The dropdown will now show "GitHub Actions" as selected
- You may see a green checkmark or "Active" indicator
- Below it, you might see a message about workflows

---

### Step 5: Verify It's Working

**Scroll down on the same page** to look for:

```
Your site is live at https://cbreiss.github.io/breisslab/
```

**If you see this:**
- ✅ Congratulations! GitHub Pages is enabled!
- Your site is being built and will be available in 2-3 minutes

**If you DON'T see this yet:**
- GitHub needs to build your site first
- Wait 2-3 minutes and refresh the page
- You should then see the message with your live URL

---

### Step 6: Check Your Website

1. Wait 2-3 minutes for the initial build
2. Click on the link: **https://cbreiss.github.io/breisslab/**
3. Your website should now be live!

---

## 🔍 Troubleshooting

### Problem: I don't see the "Settings" tab

**Solution:**
- You need to be the repository owner or have admin access
- Ask the repository owner (cbreiss) to either:
  - Enable GitHub Pages for you, OR
  - Add you as a collaborator with admin rights

---

### Problem: I don't see "Pages" in the left sidebar

**Solution:**
1. Make sure you're in the "Settings" tab (top menu)
2. Scroll down in the left sidebar - "Pages" is in the "Code and automation" section
3. If you still don't see it, refresh the page or try a different browser

---

### Problem: The dropdown only shows "Deploy from a branch"

**Solution:**
- This might mean GitHub Actions is not available for your repository
- Try selecting "Deploy from a branch" instead
- Then select:
  - Branch: `main` (or `master`)
  - Folder: `/ (root)`
- Click "Save"
- Your site should still work, but it won't use the automatic workflow

---

### Problem: "Your site is live" message doesn't appear

**Solution:**
1. Wait 2-3 minutes and refresh the Settings > Pages page
2. Check the "Actions" tab to see if the build is running
3. Look for a workflow called "pages build and deployment" or "Deploy Jekyll site to GitHub Pages"
4. If you see a red X (failed), click on it to see the error

---

### Problem: The website shows a 404 error

**Solution:**
1. Make sure you've waited at least 3 minutes after enabling Pages
2. Check that you're going to the correct URL: `https://cbreiss.github.io/breisslab/`
3. Go to Settings > Pages and verify the URL shown there
4. Check the "Actions" tab to ensure the build succeeded (green checkmark)

---

## 📸 Visual Guide

### What the Settings Tab Looks Like

When you're on the repository page, the top menu looks like this:

```
┌─────────────────────────────────────────────────────────┐
│  cbreiss / breisslab                                     │
├─────────────────────────────────────────────────────────┤
│  Code  Issues  Pull requests  Actions  ···  Settings    │  ← Click Settings
└─────────────────────────────────────────────────────────┘
```

### What the Left Sidebar Looks Like

After clicking Settings, the left sidebar shows:

```
┌──────────────────────┐
│ General              │
│ Access               │
│   Collaborators      │
│   Moderation         │
│ Code and automation  │
│   Branches           │
│   Tags               │
│   Actions            │
│   Webhooks           │
│   Environments       │
│   Pages              │  ← Click here
│   Custom properties  │
└──────────────────────┘
```

### What the Pages Settings Look Like

After clicking Pages, you'll see:

```
┌─────────────────────────────────────────────┐
│ GitHub Pages                                 │
├─────────────────────────────────────────────┤
│                                              │
│ Build and deployment                         │
│                                              │
│ Source                                       │
│ ┌───────────────────────────┐               │
│ │ GitHub Actions         ▼  │  ← Select this│
│ └───────────────────────────┘               │
│                                              │
│ Your site is live at                        │
│ https://cbreiss.github.io/breisslab/        │
│                                              │
└─────────────────────────────────────────────┘
```

---

## ✅ Success Checklist

After following these steps, you should have:

- [x] Found and clicked the "Settings" tab
- [x] Located "Pages" in the left sidebar
- [x] Selected "GitHub Actions" as the source
- [x] Seen the "Your site is live" message
- [x] Visited your website and seen it working

---

## 🎉 Next Steps

Once GitHub Pages is enabled:

1. **Wait 2-3 minutes** for the initial build
2. **Visit your site:** https://cbreiss.github.io/breisslab/
3. **Start customizing** your content (see SETUP.md)

Every time you make changes to your repository:
- GitHub will automatically rebuild your site
- Changes appear in 2-3 minutes
- No need to enable Pages again!

---

## 📞 Still Need Help?

If you're still having trouble:

1. **Check the GitHub Actions tab**
   - Click "Actions" in the top menu
   - Look for any failed builds (red X)
   - Click on them to see error details

2. **Verify your repository name**
   - Should be: `cbreiss/breisslab`
   - The URL will be: `https://cbreiss.github.io/breisslab/`

3. **Try a different approach**
   - See the "Alternative Method" section below

---

## 🔄 Alternative Method (If GitHub Actions Doesn't Work)

If you can't select "GitHub Actions", try this:

1. In Settings > Pages
2. Under "Source", select **"Deploy from a branch"**
3. Under "Branch", select **"main"** (or "master")
4. Under "Folder", select **"/ (root)"**
5. Click **"Save"**
6. Wait 2-3 minutes
7. Your site should be live!

**Note:** This method works but won't use the custom workflow. The site will still function correctly.

---

**Last Updated:** February 1, 2024

For more help, see:
- [SETUP.md](SETUP.md) - Quick setup guide
- [README.md](README.md) - Complete documentation
- [GitHub Pages Documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
