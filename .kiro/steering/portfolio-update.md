---
inclusion: manual
---

# Portfolio Audit & Update — Kiro Steering

When the user asks to audit, refresh, or update an existing technical portfolio, follow this workflow.

## Start with this message

"Let's audit and freshen up your portfolio! I'll review what you have, flag what's outdated, and help you update it.

Our process:
- 🔍 Audit — review current content for staleness and gaps
- 📋 Update Plan — prioritized list of changes
- ✏️ Implementation — make the updates
- ✅ Verification — confirm everything looks good

Which portfolio files should I look at? (Point me to your directory or list the files.)"

---

## Phase 1: Audit

Read all portfolio HTML/CSS files. For each page, check:

- **Staleness:** roles, titles, companies, or dates that appear outdated
- **Missing content:** empty sections, placeholder text, TODO comments
- **Broken links:** href values pointing to `#` or obviously dead URLs
- **Project relevance:** old projects that no longer represent current skills
- **Skills currency:** technologies listed that are no longer primary; missing newer skills
- **Design issues:** inconsistent styling, accessibility gaps (missing alt text, low contrast)
- **Mobile responsiveness:** layout problems visible in the markup

Present findings as a categorized checklist:

```
🔴 Outdated — [items needing factual updates]
🟡 Gaps — [missing or placeholder content]
🔵 Polish — [design, accessibility, or link fixes]
```

Ask the user to confirm which items to address and whether anything should be added (new projects, new role, new skills).

---

## Phase 2: Update Plan

Based on user confirmation, produce a numbered list of changes in priority order:

1. Factual corrections (role, title, company, dates)
2. New content (projects, skills, blog posts)
3. Removed content (outdated projects, old roles)
4. Link fixes
5. Design/accessibility improvements

Get approval before implementing.

---

## Phase 3: Implementation

Apply changes one file at a time. After each file:
- Show a summary of what changed
- Ask if it looks right before moving on

Order: index.html → about.html → projects.html → contact.html → blog.html → styles.css

---

## Phase 4: Verification

Guide the user to:
1. Open updated pages in a browser
2. Check mobile view
3. Click all links
4. Review overall impression

Ask: "Anything else you'd like to tweak?"

Provide a reminder to commit and push if deploying via GitHub Pages.

---

## Common requests

**Add a new project:** ask for name, description, technologies, links → add to projects.html and optionally featured section on index.html.

**Update current role:** ask for new title/company/summary → update index.html hero and about.html timeline.

**Refresh skills list:** ask what to add/remove → update about.html skills section and any skill tags on project cards.

**Remove a project:** confirm which one → remove from projects.html and index.html featured grid if present.
