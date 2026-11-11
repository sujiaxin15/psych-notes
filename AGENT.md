1. Project Overview & Purpose
- Project Name: MindPal Psychology Knowledge Hub
- Purpose: Study guide for undergraduate psychology student.
- Target Audience: Psychology students seeking fast, structured, and easy-to-read concept overviews.

2. Directory Structure & Naming Conventions
- Root directory contains `index.html` (landing page) and `AGENTS.md`.
- All sub-topic pages live inside `/pages/`.
- File naming convention for pages: lower-kebab-case (e.g., `cognitive-dissonance.html`, `classical-conditioning.html`).
- Static assets live inside `/assets/css/` and `/assets/js/`.

3. Visual Style & UI Design Guidelines
- Color Palette:
  - Primary Accent: Indigo Blue (`#4F46E5`)
  - Secondary Accent: Emerald Green (`#10B981`)
  - Background: Off-white (`#F9FAFB`)
  - Card Background: Pure White (`#FFFFFF`)
  - Text Primary: Dark Charcoal (`#1F2937`)
  - Text Secondary: Cool Gray (`#6B7280`)
- Typography: System sans-serif font stack (`system-ui, -apple-system, sans-serif`).
- Layout: Centered container max-width `900px` with clean card components and subtle shadows (`box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1)`).

4. Standard Page Template & Required Sections
Every new topic page inside `/pages/` MUST strictly contain the following section structure:
1. Header Navigation: Back link to `../index.html` + Page Title.
2. Concept Summary Card: High-level 2-sentence definition.
3. Core Elements (List/Grid): 3–4 essential components or mechanisms.
4. Real-Life Analogy Box: A relatable scenario illustrating the concept.
5. Key Terms Glossary Table: Columns for `Term` | `Definition` | `Example`.
6. Footer: Standard navigation links and copyright notice.

5. Rules for AI Modifying or Adding Content
When asked to create a new page or edit existing content, AI MUST follow these steps:
1. Create File: Save the new page under `/pages/topic-name.html` using the template format.
2. Update Index: Automatically add a card link for the new page on `index.html` under the appropriate category grid.
3. Navigation Integrity: Ensure all relative link paths (`../index.html` vs `./pages/...`) are correct.
4. Design Consistency: Do NOT write custom inline CSS style tags; reuse existing CSS classes from `assets/css/style.css`.
