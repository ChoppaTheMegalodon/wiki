---
title: Images
draft: true
---

# images/

General image library for the wiki — diagrams, screenshots, headshots, OG images, page headers, decorative assets.

**This folder is for wiki-page imagery, not memes.** Memes live in [[../memes/index|memes/]] (separate folder with WIP/Done structure).

## Usage

Drop images into this folder and reference them from any page:

```markdown
![alt text](../images/diagram.png)
![[diagram.png]]     # Obsidian-style embed, also works in Quartz
```

Subfolders are fine if it gets messy (`images/diagrams/`, `images/headshots/`, etc).

## Conventions

- Prefer `.webp` or `.png` for diagrams/screenshots
- Prefer `.jpg` for photos
- Filename: lowercase-kebab-case, no spaces (`flywheel-diagram.png`, not `Flywheel Diagram.png`)
- If an image is used on only one page, consider co-locating it with that page instead of here
