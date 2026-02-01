# Content Update Guide for Breiss Lab Website

This guide provides templates and examples for common website updates.

## Table of Contents
1. [Adding a News Post](#adding-a-news-post)
2. [Adding a Team Member](#adding-a-team-member)
3. [Adding a Publication](#adding-a-publication)
4. [Adding a Research Area](#adding-a-research-area)
5. [Formatting Tips](#formatting-tips)

---

## Adding a News Post

### Step 1: Create the file
Create a new file in the `_posts/` folder named: `YYYY-MM-DD-title.md`

Example: `2024-03-15-new-paper-published.md`

### Step 2: Use this template

```markdown
---
title: "Title of Your News Post"
date: 2024-03-15
categories:
  - News
  - Research
tags:
  - publications
  - awards
---

Write your news content here.

You can include:
- Multiple paragraphs
- Links to [publications](url)
- Images ![description](/breisslab/assets/images/photo.jpg)

## Subsections

Add more details with subsections.
```

### Examples of News Posts:

**New Publication:**
```markdown
---
title: "New Paper Published in Nature"
date: 2024-03-15
categories:
  - Publications
tags:
  - research
---

We're excited to announce that our latest research has been published in Nature!

Read the paper: [Link to DOI](https://doi.org/xxx)
```

**Grant Award:**
```markdown
---
title: "Lab Awarded NSF Grant"
date: 2024-03-20
categories:
  - News
  - Funding
tags:
  - grants
---

We're pleased to announce that we've been awarded a 3-year grant from the National Science Foundation...
```

**New Team Member:**
```markdown
---
title: "Welcome Our New Postdoc!"
date: 2024-04-01
categories:
  - People
tags:
  - team
---

Please join us in welcoming Dr. Jane Smith to the lab! Dr. Smith will be working on...
```

---

## Adding a Team Member

### Edit `_pages/people.md`

**For a Postdoc:**
```markdown
<div style="margin-bottom: 30px;">
  <h3>Dr. Jane Smith</h3>
  <p><strong>Postdoctoral Researcher</strong></p>
  <p>
    Dr. Smith received her Ph.D. from MIT in 2023. Her research focuses on 
    computational biology and machine learning applications in genomics.
  </p>
  <p>
    <a href="mailto:jsmith@breisslab.edu">📧 Email</a> | 
    <a href="https://scholar.google.com/citations?user=xxx">🎓 Google Scholar</a>
  </p>
</div>
```

**For a Graduate Student:**
```markdown
<div style="margin-bottom: 30px;">
  <h3>John Doe</h3>
  <p><strong>Ph.D. Candidate</strong></p>
  <p>
    John is investigating the role of protein interactions in cellular signaling. 
    He joined the lab in 2021.
  </p>
  <p><a href="mailto:jdoe@university.edu">📧 Email</a></p>
</div>
```

**For an Undergraduate:**
```markdown
- **Sarah Johnson** - Working on CRISPR screening experiments (started Fall 2023)
```

---

## Adding a Publication

### Edit `_pages/publications.md`

Add under the appropriate year section:

```markdown
### 2024

1. **Smith J**, Doe J, **Johnson S**, Brown A (2024). "Title of Your Paper." *Journal Name*, Volume(Issue), pages. [DOI](https://doi.org/10.xxxx/xxxxx) | [PDF](/breisslab/assets/pdfs/smith2024.pdf)
```

**Format notes:**
- Use `**Name**` for lab members (makes them bold)
- Include DOI link
- Optionally add PDF link if you have the file in `assets/pdfs/`
- List authors in order as they appear on the paper

**For a preprint:**
```markdown
## Preprints

- **Smith J**, Doe J (2024). "Preprint Title." *bioRxiv*. [DOI](https://doi.org/10.1101/2024.xx.xx.xxxxxx)
```

---

## Adding a Research Area

### Edit `_pages/research.md`

Use this template:

```markdown
### Research Area: [Your Topic]

[2-3 paragraphs describing this research area]

Our approach combines [methods] to address [scientific questions]. We collaborate with [collaborators] and use techniques including [techniques].

**Key Publications:**
- Author et al. (2024). "Paper title." *Journal*. [DOI](link)
- Author et al. (2023). "Paper title." *Journal*. [DOI](link)

**Funding:**
- NIH R01 Grant (2022-2027)
- NSF CAREER Award (2021-2026)

**Current Projects:**
- Project 1: [Brief description]
- Project 2: [Brief description]

---
```

---

## Formatting Tips

### Basic Markdown

| What you type | What you get |
|--------------|--------------|
| `# Heading 1` | Large heading |
| `## Heading 2` | Medium heading |
| `### Heading 3` | Small heading |
| `**bold**` | **bold** |
| `*italic*` | *italic* |
| `[text](url)` | Clickable link |
| `- item` | Bullet point |
| `1. item` | Numbered list |

### Adding Links

```markdown
[Link text](https://url.com)
[Email](mailto:email@domain.com)
```

### Adding Images

```markdown
![Alt text for accessibility](/breisslab/assets/images/filename.jpg)
```

**Important:** 
1. Upload image to `assets/images/` first
2. Use the full path starting with `/breisslab/`
3. Use descriptive alt text for accessibility

### Adding Email Links

```markdown
[📧 Email](mailto:name@email.com)
```

### Line Breaks

- Single line break: Just hit Enter once (creates new line in same paragraph)
- Paragraph break: Hit Enter twice (creates new paragraph with space)
- Horizontal line: Use `---` on its own line

### Special Characters

You can use emojis directly:
- 📧 `:email:`
- 🎓 `:mortar_board:`
- 🔬 `:microscope:`
- 📄 `:page_facing_up:`
- 🌐 `:globe_with_meridians:`

---

## Quick Reference: File Locations

| Content Type | File Location |
|--------------|---------------|
| Home page | `index.md` |
| Research | `_pages/research.md` |
| People | `_pages/people.md` |
| Publications | `_pages/publications.md` |
| Contact | `_pages/contact.md` |
| News posts | `_posts/YYYY-MM-DD-title.md` |
| Images | `assets/images/` |
| PDFs | `assets/pdfs/` |
| Site settings | `_config.yml` |
| Navigation menu | `_data/navigation.yml` |

---

## Checklist Before Publishing Changes

- [ ] Preview your changes (if running locally)
- [ ] Check all links work
- [ ] Verify image paths are correct
- [ ] Check spelling and grammar
- [ ] Ensure formatting looks correct
- [ ] Test on mobile (after deploying)
- [ ] Update the date if it's a news post

---

## Getting Help

If you're stuck:
1. Check the main README.md for setup instructions
2. Look at existing files for examples
3. Consult the [Markdown Guide](https://www.markdownguide.org/)
4. Check [Minimal Mistakes documentation](https://mmistakes.github.io/minimal-mistakes/)
5. Open an issue on GitHub if you need help

---

**Last Updated:** February 1, 2024
