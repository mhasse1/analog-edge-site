# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for Analog Edge, a technology transformation consulting firm. The site is a single-page portfolio showcasing the company's philosophy, results, and contact information. The project is primarily a static HTML site with embedded CSS and no build process.

## Repository Structure

- `index.html` - Main landing page with complete site content and embedded CSS
- `materials/` - Marketing materials and design assets (business cards, brochures, logo variants)  
- `images/` - Logo files and design assets in various formats (PNG, SVG, PXD files)
- `MarkHasseResume.pdf` - Resume document
- `CNAME` - GitHub Pages domain configuration
- `LICENSE` - Project license

## Development Commands

This is a static HTML site with no build process. No package.json, npm scripts, or build tools are configured.

**To develop locally:**
- Open `index.html` directly in a browser, or
- Use any static file server (e.g., `python -m http.server`, `live-server`, etc.)

**For GitHub Pages deployment:**
- Changes to `main` branch are automatically deployed via GitHub Pages
- Domain configured via `CNAME` file

## Architecture Notes

**Single-page application:**
- All content, styling, and animations are contained in `index.html`
- CSS is embedded in `<style>` tags (no external stylesheets)
- No JavaScript frameworks or external dependencies
- Pure CSS animations for visual effects (particles, gradients, waves)

**Content sections:**
- Hero section with animated logo and company philosophy
- Results showcase with metrics cards
- Transformation stories highlighting past successes  
- Contact section with obfuscated email and multiple contact methods

**Design system:**
- Gradient color scheme (green/cyan/blue)
- Responsive grid layout with mobile breakpoints
- Animated elements representing "analog to digital" transformation
- Professional consulting aesthetic with tech-forward visual effects

## Content Management

The site content is directly embedded in the HTML. To update:
- Company information: Edit text content in respective sections
- Contact details: Update contact-info section (line ~821)
- Case studies: Modify story-cards content (line ~783)
- Metrics: Update result-card numbers and descriptions (line ~748)

Email is obfuscated using JavaScript to prevent spam harvesting (line ~833).