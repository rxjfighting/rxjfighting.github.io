# Homepage

This repository contains my personal homepage, built with Jekyll and deployed through GitHub Pages.

## What this site uses

- Jekyll for site generation
- `_config.yml` for site settings
- `_pages/about.md` for the homepage content
- `_includes/` and `_layouts/` for shared templates
- `_sass/` and `assets/css/` for styling
- `google_scholar_crawler/` for scholar statistics updates

## Quick update guide

If I want to change the homepage later, the usual files to edit are:

- `_pages/about.md`: homepage text and sections
- `_config.yml`: title, author info, social links, analytics, SEO settings
- `_data/navigation.yml`: top navigation items
- `_includes/`: header, footer, sidebar, and reusable page fragments
- `_sass/`: theme and layout styles
- `assets/js/`: custom scripts

## Local development

1. Install Ruby and Bundler.
2. Install dependencies with `bundle install`.
3. Start the local server with:

```bash
bash run_server.sh
```

4. Open `http://127.0.0.1:4000` in a browser.

The server supports live reload, so most changes should appear automatically after saving files.

## Debug checklist

If something looks broken, check these first:

- Make sure the Jekyll server is still running without errors.
- Confirm the edited markdown file is included by `_config.yml`.
- Check the browser console for JavaScript errors.
- Check the terminal for Liquid, Markdown, or Sass build errors.
- If styles look wrong, rebuild or refresh after editing files under `_sass/` or `assets/css/`.
- If scholar stats do not update, verify the crawler settings and GitHub Actions workflow.