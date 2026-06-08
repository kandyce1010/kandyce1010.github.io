---
inclusion: manual
---

# Technical Portfolio Builder — Kiro Steering

When the user asks for help building or updating a technical portfolio, follow this guided workflow.

## Start with this message

"Welcome to the Technical Portfolio Builder! I'll guide you through creating a professional portfolio website.

Our process:
- 📋 Information Gathering — collect your professional details
- 🎨 Design Preferences — choose your style
- 🏗️ Portfolio Generation — create your complete website
- ✅ Review & Refinement — polish and deploy

Let's begin!"

---

## Phase 1: Information Gathering

Collect the following, one step at a time. Always wait for a response before proceeding.

**Step 1 — Basic info:** full name, current role, professional summary (2-3 sentences), years of experience, 5-7 primary skills.

**Step 2 — Career:** current company/role, previous 2-3 roles, key milestones, specializations.

**Step 3 — Projects (3-5):** name, description, technologies, problem/impact, GitHub link, demo link.

**Step 4 — Links:** LinkedIn, GitHub username, email, other professional links.

**Step 5 — Design:** color preferences, inspiration examples, professional photo available?

Confirm all collected before Phase 2.

---

## Phase 2: Structure Planning

Summarize collected info, flag any gaps, then propose and get approval for:

```
Homepage    — hero, summary, top 3 projects
About       — career timeline, skills, background
Projects    — detailed project cards
Blog        — optional
Contact     — links and contact method
```

---

## Phase 3: Generation

Use templates from `templates/` directory as the base. Fill in real user content.

Order: index.html → about.html → projects.html → contact.html → blog.html (if applicable) → styles.css (apply color scheme).

Show generated files and ask for review.

---

## Phase 4: Review & Refinement

Guide the user to test in browser (all pages, mobile view, all links). Gather feedback. Implement one change at a time. Then provide GitHub Pages deployment steps.

---

## Principles

- Content first — real info, minimal placeholders
- WCAG accessibility — alt text, color contrast, semantic HTML
- Mobile-first responsive
- If short on time: 3 core pages (home, about, projects), skip blog

---

## Common requests

**Add a project:** ask for name, description, technologies, links → add card to projects.html and optionally index.html featured grid.

**Change colors:** ask for preferred color → update gradient and accent in styles.css.

**Fix a link:** ask for correct URL → find and update.

**Run short on time:** focus on 3 core pages, use template colors, note what to refine later.
