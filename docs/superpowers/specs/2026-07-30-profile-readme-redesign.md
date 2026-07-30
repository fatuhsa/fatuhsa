# Design Spec: GitHub Profile README Redesign (fatuhsa)

Date: 2026-07-30
Author: Antigravity & fatuhsa
Status: Approved

## 1. Goal & Aesthetic Direction
- **Goal**: Clean up and modernize the GitHub profile README for user `fatuhsa`.
- **Aesthetic Theme**: Modern Aesthetic Weeb (Dark Purple `#9f7aea` accent, clean typography, badge grouping, animated stats, and contribution snake).

## 2. Layout Structure

### Header
- Centered header banner with aesthetic anime gif and profile visitor counter badge (`orang yang ngintip`).
- Clean separator lines (`---`).

### About Me
- Structured text without emojis:
  - Weeb developer crafting code for fun and passion.
  - Primary stack: Frontend (Svelte, React, Vue), Backend (Node.js), TypeScript/JavaScript ecosystem.
  - Always learning and experimenting with new web technologies.

### Tech Stack
- Categorized badges into distinct groups using `for-the-badge` style (no Python):
  - **Frontend**: Svelte, React, Vue.js, Tailwind CSS
  - **Languages & Backend**: TypeScript, JavaScript, Node.js
  - **Tools**: Vite, Git, GitHub Actions

### GitHub Analytics & Stats
- **GitHub Readme Stats Card**: Shows total stars, commits, PRs, issues, and rank (Theme: `tokyonight` or `radical`).
- **Most Used Languages Card**: Top languages breakdown.
- **GitHub Streak Stats**: Daily commit streak tracking.

### Contribution Snake Animation
- Displays the generated snake animation SVG (`dist/github-contribution-grid-snake.svg`) in a dedicated centered block.

### Footer & Socials
- Clean links/badges for GitHub profile and social presence.

## 3. Workflow & CI Integration
- Retain `.github/workflows/snake.yml` which generates `dist/github-contribution-grid-snake.svg` every 6 hours and updates the repo.

## 4. Acceptance Criteria
- README render is clean, visual hierarchy is well organized, badges look uniform and high quality.
- Markdown syntax is completely valid without broken links or broken image tags.
- Snake animation SVG reference points to the correct relative/absolute path.
