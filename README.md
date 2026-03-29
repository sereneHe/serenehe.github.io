# Xiaoyu He Personal Website

This repository contains the source code for Xiaoyu He's academic website:

- Live site: https://serenehe.github.io/

The site is built with Hugo and Hugo Blox, and deployed to GitHub Pages through GitHub Actions.

## Site Structure

- `content/authors/admin/`: homepage profile, biography, education, and skills
- `content/publication/`: publication entries
- `content/project/`: project entries
- `content/_index.md`: homepage section configuration
- `content/experience.md`: experience page configuration
- `config/_default/`: site title, base URL, menus, and Hugo settings
- `.github/workflows/publish.yaml`: GitHub Pages build and deployment workflow

## Local Development

Run the site locally from the repository root:

```bash
hugo server
```

If Hugo modules need to be refreshed, run:

```bash
hugo mod tidy
```

## Deployment

Deployment is automatic on pushes to `main`.

The GitHub Pages workflow:

- builds the site with Hugo `0.136.5`
- generates the Pagefind search index
- deploys the `public/` output to GitHub Pages

## Main Sections

- Home
- Publications
- Experience
- Projects

## Notes

- The production `baseURL` is set to `https://serenehe.github.io/`
- Project and publication cards use images placed alongside each entry in `content/`
- Some homepage presentation tweaks are implemented through custom layout overrides in `layouts/`
