---
description: Add a new project card to the portfolio. Asks for project details then inserts the HTML into projects.html and optionally index.html.
---

Add a new project card to the portfolio.

Ask me for the following details (ask all at once):
- Project name
- What problem it solved / what it does (2-3 sentences)
- Technologies used (list them)
- Link to GitHub repo or live demo (or both)
- Should this be featured on the homepage too? (yes/no)

Once I provide the details:
1. Add a `.project-card` to `projects.html` inside the `.projects-grid` — most recent work first
2. If featured: also add a card to the `.projects-grid` in `index.html` (keep featured to 3-4 max — if already at 4, ask which one to replace)
3. Match the existing card structure exactly — `<h3>`, `<p>`, `.project-tech` with `.tech-tag` spans, `.project-link`

Don't invent details I didn't provide. Use placeholder text only where I explicitly say to.
