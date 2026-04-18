# Deployment Guide

## Overview

This document describes how the WMDC Consensus website is automatically deployed using GitHub Actions.

## Deployment Process

### Automatic Deployment

The website automatically deploys when:

1. **Push to Main Branch** - Code merged to `main` triggers deployment
2. **Documentation Changes** - Changes to `docs/` or markdown files
3. **Manual Trigger** - Workflow can be run manually from Actions tab

### Workflow Steps

1. **Checkout** - Downloads repository code
2. **Setup Hugo** - Installs Hugo Extended 0.124.0
3. **Build** - Generates static HTML with `hugo --minify`
4. **Upload Artifact** - Stores built files as GitHub artifact
5. **Deploy** - Publishes artifact to GitHub Pages

## Manual Deployment

### Option 1: GitHub Actions

1. Go to **Actions** tab
2. Select **Deploy Website** workflow
3. Click **Run workflow**
4. Select branch and click **Run workflow**

### Option 2: Local Build

```bash
cd docs
hugo --minify
# Upload docs/public/ to hosting
```

## GitHub Pages Configuration

### Settings

1. Go to repository **Settings**
2. Navigate to **Pages** in sidebar
3. Configure:
   - **Source**: GitHub Actions
   - **Branch**: No selection needed (uses workflow)

## Troubleshooting

### Build Failures

1. Check Hugo version compatibility
2. Verify all theme files exist
3. Check for Markdown syntax errors

### Deployment Failures

1. Ensure GitHub Pages is enabled
2. Check workflow permissions
3. Verify no concurrent deployments

### Preview Locally

```bash
cd docs
hugo server -D  # Include drafts
```

## Permissions

The workflow requires these GitHub permissions:

```yaml
permissions:
  contents: read      # Read repository
  pages: write       # Deploy to Pages
  id-token: write    # Authenticate
```

---

*For issues, open a GitHub Discussion or Issue.*
