# Kandyce Bohannon — Personal Portfolio

This is a static HTML/CSS portfolio deployed to GitHub Pages at https://kandyce1010.github.io.
No build step, no frameworks — just files pushed to `main` and served directly.

## File structure

```
index.html                  Homepage — hero, featured work, speaking banner
about.html                  Career timeline, skills, speaking/community section
projects.html               Detailed project cards
blog.html                   Blog post grid
contact.html                Contact methods and links
she-builds-episodes.html    Video content — She Builds episodes + other livestream appearances
amazon-q-developer-journey.html  Deep-dive page on Q Developer work (may be stale)
styles.css                  All styles — shared across every page
images/                     Photos and event images
.amazonq/                   Amazon Q CLI task tracking (legacy — can be ignored)
```

## Design system

**Color palette:**
- Primary gradient: `#ec4899` (pink) → `#8b5cf6` (purple) — used in hero sections and banners
- Accent: `#c026d3` (fuchsia) — used for timeline years, arrow bullets, CTAs
- Text dark: `#1e293b`
- Text muted: `#64748b`
- Background light: `#f8fafc`
- Border: `#e2e8f0`

**Nav:** Fixed header, hamburger on mobile. Active page gets `class="active"` on its `<li><a>`. Nav order: Home → About → Projects → Video Content → Blog → Contact.

**Styles live in `styles.css` for shared rules.** Page-specific overrides are sometimes inlined in `<style>` tags at the bottom of the file — that's intentional for pages that diverge from the base.

**Components:**
- `.project-card` — white card with shadow, tech tags (`.tech-tag`), project link
- `.timeline-item` — grid: year column + content column; year in accent color
- `.tech-item` — gray pill in the skills grid
- `.btn.btn-primary` / `.btn.btn-secondary` / `.btn.btn-accent` — CTA buttons
- `.reinvent-banner` / `.banner-content` — image + text side by side for event promos

## Common tasks

### Add a project card (to projects.html or index.html featured grid)
Each card follows this structure:
```html
<div class="project-card">
    <h3>Project Name</h3>
    <p>2-3 sentence description. What problem, what solution, what impact.</p>
    <div class="project-tech">
        <span class="tech-tag">Tag1</span>
        <span class="tech-tag">Tag2</span>
    </div>
    <a href="URL" class="project-link">Link text →</a>
</div>
```

### Add a blog post entry (to blog.html)
```html
<div class="blog-card">
    <div class="blog-meta">
        <span class="blog-date">Month YYYY</span>
        <span class="blog-category">Category</span>
    </div>
    <h3>Post Title</h3>
    <p>2-3 sentence excerpt.</p>
    <div class="blog-tags">
        <span class="tech-tag">Tag</span>
    </div>
    <a href="URL" class="project-link">Read More →</a>
</div>
```

### Add a video/livestream entry (to she-builds-episodes.html)
Match the existing card pattern in that file — date, show name, episode title, description, YouTube link.

### Update the career timeline (in about.html)
Each entry:
```html
<div class="timeline-item">
    <div class="timeline-year">YEAR</div>
    <div class="timeline-content">
        <h4>Role — Company</h4>
        <p>One sentence on what you did and the domain.</p>
    </div>
</div>
```
Timeline is in reverse-chronological order (most recent first).

### Update speaking/events
The re:Invent banner section in `index.html` and `about.html` is a promo block. Once an event has passed, convert it to a past-speaking entry in the `speaking-grid` on `about.html` rather than a banner.

## Deployment

```bash
git add <files>
git commit -m "message"
git push origin main
```

GitHub Pages serves `main` automatically. Changes are live within ~30 seconds.

## Conventions

- Keep page-level `<style>` blocks at the bottom of the `<body>` (before `</body>`), not in `<head>`
- `toggleMobileMenu()` script is duplicated in each file's inline `<script>` — keep it there
- Alt text on all images (WCAG)
- Footer text: `&copy; 2025 Kandyce Bohannon. All rights reserved.` — update year as needed
