# Entreluma project website

The promotional site at https://entreluma.org, created from [rsnyder/entreluma](https://github.com/rsnyder/entreluma). This repository owns the project branding, homepage, About page, getting-started guide, and search/social metadata.

Use **rsnyder/entreluma** to create a new storytelling site. Do not use this promotional repository as your template. The optional editor is maintained in [rsnyder/entreluma-editor](https://github.com/rsnyder/entreluma-editor).

The homepage introduces the framework, while `/examples/` renders the site's `_posts` collection with the standard Entreluma post index. This separation uses the same layouts and includes shipped by the template; only the project copy and `assets/css/custom.css` are site-specific.

## Publishing

GitHub Actions builds Jekyll and deploys to GitHub Pages. The custom domain is configured in this repository’s Pages settings. The workflow derives deployment URL and repository identity from those settings. No domain change is needed in Cloudflare when moving between repositories owned by rsnyder.

## Local development

Use the Ruby version in `.ruby-version`, then run `bundle install` and `bundle exec jekyll serve`. Run the consistency, local media, and internal-link checks used by `.github/workflows/pages-deploy.yml` before publishing changes.

## Updating the shared runtime

This is an independent copy, not a fork or automatically synchronized dependency. Apply selected template improvements with review, keeping this repository’s branding and content. Changes useful to all publishers should first be made in the template. Never copy this site’s public identity, analytics IDs, verification codes, or promotional content back into template defaults.
