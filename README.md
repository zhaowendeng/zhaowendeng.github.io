# Zhaowen Deng's academic website

This site uses GitHub Pages and Jekyll. The blue banner, portrait sidebar, and page layout are shared across Home, Publication, Conference, and CV. Content updates do not require editing the layout.

## Edit on GitHub

1. Open a file in this repository and click the pencil icon.
2. Make the change and click **Commit changes**. GitHub Pages will publish it automatically after the build finishes.

| Change | File to edit |
| --- | --- |
| Name, affiliation, email, links, education, experience, or footer date | `_data/profile.yml` |
| Replace the portrait | `profile.png` (keep the same filename) |
| Edit a publication | Its file in `_publications/` |
| Add a publication | Create another `.md` file in `_publications/` |
| Add a conference item | Create a `.md` file in `_conferences/` |
| Add a project item | Create a `.md` file in `_projects/` |

For a new publication, conference item, or project, copy this example into a new Markdown file in the appropriate folder:

```md
---
title: "Title of the work"
order: 3
---
Authors. *Venue* (Year). [Link](https://example.com/)
```

For publications, give each new item the next larger `order` number (for example, 3 after 2). Publications display in descending order, so the newest item appears first on Publication, Home, and CV; existing files need no renumbering. Conference and project items still display in ascending `order`. Text below the second `---` uses ordinary Markdown. Empty Conference and Project sections have no placeholder text.

The shared design and navigation live in `_layouts/default.html`. The short page files `index.html`, `publication.md`, `conference.md`, and `cv.md` select which sections to display.
