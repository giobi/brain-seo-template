# Brain SEO Template - Mission & Usage Guide

## Mission

**Brain SEO Template** is a Git-based repository structure for managing SEO content, keyword research, competitor analysis, and technical audits in a structured, version-controlled way.

**Why this template?**
- Replace scattered spreadsheets and Notion pages
- Track SEO strategy evolution with Git commits
- AI-friendly markdown format (ChatGPT, Claude, Gemini, etc.)
- Human-readable, searchable, portable

**Who is this for?**
- SEO managers and consultants
- Content strategists
- Marketing teams managing multiple clients/projects
- Anyone who wants organized, version-controlled SEO workflows

---

## Quick Start

### 1. Clone this template

```bash
git clone https://github.com/giobi/brain-seo-template.git my-seo-brain
cd my-seo-brain
rm -rf .git  # Remove template git history
git init     # Start your own repo
```

### 2. Open in VSCode

```bash
code .
```

### 3. Start adding content

Use the examples in each folder as templates. Copy, rename, and customize them for your projects.

---

## Folder Structure

```
brain-seo-template/
├── keywords/        # Keyword research and analysis
├── content/         # Blog posts, landing pages, content briefs
├── competitors/     # Competitor analysis and monitoring
├── backlinks/       # Link building strategy and outreach
├── technical/       # Technical SEO audits and fixes
├── reports/         # Monthly/weekly SEO reports
└── projects/        # Client or site-specific projects
```

Each folder contains a `.index.md` file explaining what goes inside and an example file to get you started.

---

## How to Use This with AI Assistants

### With ChatGPT / Claude / Gemini

This repository is designed to work seamlessly with AI assistants. Here's how:

**1. Ask AI to create content:**
```
"Create a keyword research file for 'sustainable fashion' in the keywords/ folder"
```

**2. Ask AI to analyze existing files:**
```
"Read all files in competitors/ and summarize the main threats"
```

**3. Ask AI to generate reports:**
```
"Create a monthly SEO report in reports/ based on the last 30 days of content in content/"
```

**4. Ask AI to organize projects:**
```
"Create a new project folder for client XYZ in projects/ with keyword research, content plan, and technical audit"
```

### With Claude Code (Advanced)

If you're using Claude Code (Anthropic's CLI), you can:
- Run agents to automate workflows
- Use Git hooks for validation
- Integrate with external APIs (Google Search Console, SEMrush, Ahrefs, etc.)

But **this template is designed to work WITHOUT Claude Code**. You can use it with any AI assistant + VSCode + Git.

---

## Workflow Examples

### Example 1: New Blog Post

1. Research keywords in `keywords/`
2. Create content brief in `content/drafts/`
3. Write post in `content/posts/`
4. Commit changes: `git commit -m "Add blog post: SEO best practices 2025"`

### Example 2: Competitor Analysis

1. Create competitor file in `competitors/`
2. Document their top pages, keywords, backlinks
3. Identify gaps and opportunities
4. Reference in your content strategy

### Example 3: Technical Audit

1. Create audit file in `technical/`
2. List issues (broken links, slow pages, missing meta tags)
3. Track fixes with Git commits
4. Generate report in `reports/`

### Example 4: Client Project

1. Create folder in `projects/client-name/`
2. Add subfolders: `keywords/`, `content/`, `technical/`
3. Centralize all client SEO work in one place
4. Share via Git (GitHub, GitLab, Bitbucket)

---

## File Naming Conventions

**Use lowercase + hyphens:**
- ✅ `sustainable-fashion-keywords.md`
- ❌ `Sustainable Fashion Keywords.md`

**Use dates for time-based files:**
- ✅ `2025-11-monthly-report.md`
- ✅ `2025-11-21-blog-post-seo-trends.md`

**Use descriptive names:**
- ✅ `competitor-analysis-example-com.md`
- ❌ `comp1.md`

---

## Markdown Best Practices

**Use frontmatter for metadata:**

```markdown
---
title: Sustainable Fashion Keywords
date: 2025-11-21
status: research
tags: [fashion, sustainability, ecommerce]
---

# Sustainable Fashion Keywords

...
```

**Use tables for data:**

```markdown
| Keyword | Volume | Difficulty | Intent |
|---------|--------|------------|--------|
| sustainable fashion | 12,000 | 65 | Informational |
| eco-friendly clothing | 8,000 | 55 | Commercial |
```

**Use links to connect files:**

```markdown
See competitor analysis: [Example.com](../competitors/example-com.md)
```

---

## Git Workflow

**Commit often:**
```bash
git add .
git commit -m "Add keyword research for Q4 campaign"
git push
```

**Use branches for experiments:**
```bash
git checkout -b new-content-strategy
# Make changes
git checkout main
git merge new-content-strategy
```

**Use tags for milestones:**
```bash
git tag -a "2025-Q4-launch" -m "Q4 campaign launch"
git push --tags
```

---

## Customization

**Add your own folders:**
- `analytics/` - Google Analytics reports
- `social/` - Social media SEO
- `local/` - Local SEO (Google Business Profile)
- `ecommerce/` - Product SEO for online stores

**Add your own tools:**
- Python scripts for data analysis
- API integrations (Search Console, Ahrefs, SEMrush)
- Automation with Zapier/Make

**But keep it simple:**
- Start with the core folders
- Add complexity only when needed
- Markdown-first approach

---

## Tips for Transitioning from ChatGPT/Spreadsheets

### From ChatGPT to This Repo

**Before:**
```
You: "Give me 20 keywords for sustainable fashion"
ChatGPT: [lists keywords]
You: [copies to spreadsheet]
```

**After:**
```
You: "Create a keyword research file in keywords/ for sustainable fashion with 20 keywords in a table"
AI: [creates keywords/sustainable-fashion.md with structured data]
You: git commit -m "Add sustainable fashion keywords"
```

**Benefits:**
- Versioned history (see what changed over time)
- Structured format (easy to search and reference)
- Shareable (send Git repo link to team)
- AI-readable (AI can read existing files and build on them)

### From Spreadsheets to Markdown

**Spreadsheet:**
```
| Keyword | Volume | Difficulty |
```

**Markdown:**
```markdown
---
title: Fashion Keywords
date: 2025-11-21
---

# Fashion Keywords

| Keyword | Volume | Difficulty | Notes |
|---------|--------|------------|-------|
| sustainable fashion | 12K | 65 | High intent |
```

**Benefits:**
- Markdown supports rich text (bold, links, code blocks)
- Easier to version control than Excel/Sheets
- Portable (works in any text editor)

---

## FAQ

**Q: Do I need Claude Code to use this?**
A: No. This works with any AI assistant (ChatGPT, Claude, Gemini) + VSCode + Git.

**Q: Can I use this without AI?**
A: Yes. It's just a folder structure with markdown files. Use it however you want.

**Q: Can I share this with my team?**
A: Yes. Push to GitHub/GitLab and invite collaborators.

**Q: Can I use this for multiple clients?**
A: Yes. Create a folder per client in `projects/` or create separate repos per client.

**Q: Can I customize the structure?**
A: Absolutely. Add/remove folders as needed. This is a starting template.

**Q: What if I don't know Git?**
A: Learn the basics:
- `git add .` - Stage changes
- `git commit -m "message"` - Save changes
- `git push` - Upload to GitHub
- That's 90% of what you need.

---

## Support & Feedback

This template is maintained by [@giobi](https://github.com/giobi).

**Issues/Suggestions:** https://github.com/giobi/brain-seo-template/issues

**Template version:** 1.0.0 (2025-11-21)

---

## License

MIT License - Use freely, modify, share.

---

**Now go build your SEO brain. Happy optimizing!**
