---
layout: page
title: Get started with Entreluma
permalink: /getting-started/
description: Create an interactive storytelling site from the Entreluma GitHub template, customize it, and publish your first Markdown story on GitHub Pages.
---

Create your own site from the Entreluma template, then publish a story using Markdown and interactive viewers. You need a GitHub account and a repository where GitHub Pages is available.

## 1. Create your repository

Use [the Entreluma template](https://github.com/rsnyder/entreluma/generate) to create a repository under your account. Choose a name for your project. A public repository is the simplest starting point for GitHub Pages.

## 2. Enable GitHub Pages

Open your new repository’s **Settings → Pages**. Under **Build and deployment**, select **GitHub Actions**. The initial workflow waits briefly for this setting. If it has already finished without deploying, open **Actions → Build and Deploy → Run workflow**.

After the deployment succeeds, GitHub shows the published URL in Pages settings. The workflow configures the site’s URL and repository identity automatically, including project subpaths.

## 3. Make it yours

Edit `_config.yml` to set your title, tagline, description, and optional author or organization details. Replace the introduction in `index.html` and the text in `_tabs/about.md`. The template does not include this promotional site’s identity, custom domain, analytics, or verification codes.

## 4. Write your first story

Copy `_posts/.template.md` to `_posts/YYYY-MM-DD-your-story.md`, using your publication date. Set a title and description in its YAML header and set `published: true` when ready. Write the body in Markdown.

Keep story media in a folder such as `assets/posts/your-story/`. The [author guide]({{ '/admin/' | relative_url }}) explains how to add viewers, link prose to image regions or map locations, and choose a reading layout.

## 5. Publish and check

Commit your changes to your repository’s default branch. GitHub Actions builds and deploys the site. Open the published story and check its links, images, and interactive viewers on desktop and mobile.

## Choose your editor

Use GitHub’s web interface or any Markdown editor. The optional [Entreluma Editor](https://editor.entreluma.org) adds live preview and GitHub sync. GitHub sign-in is needed only when using its GitHub features; it is not required to read a published site.

## Help readers find your work

Give each story a useful title and description, link to it from your homepage, and submit your site’s `sitemap.xml` through Google Search Console. Set up a custom domain in your repository’s Pages settings if you want one.
