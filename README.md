# GentleVale Care Website

A static marketing website for GentleVale, a domiciliary care service based in Welwyn Garden City.

## Portfolio overview

A responsive HTML/CSS/JavaScript site with service information, contact navigation, search metadata and automated static-site deployment. This repository demonstrates small-business website implementation and deployment configuration.

## Features

- Responsive single-page site.
- Service, approach, coverage, and contact sections.
- SEO metadata, sitemap, robots file, and favicon.
- Cloudflare Pages deployment workflow.

## Tech Stack

- HTML
- CSS
- JavaScript
- GitHub Actions
- Cloudflare Pages

## Deployment

The site is configured for Cloudflare Pages. See `DEPLOYMENT.md` for the required repository secret and deployment setup.

The deployment workflow copies the static site files into `.deploy/` and publishes them on pushes to `main`.
