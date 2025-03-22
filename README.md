# New Religions Website Documentation

This is a Jekyll-based static website hosted on GitHub Pages. This document contains instructions for transferring repository ownership and maintaining the website.

## Repository Transfer Process

### Option 1: Direct Repository Transfer (Recommended)
1. Once the client has created their GitHub account:
   - Go to repository Settings
   - Scroll to "Danger Zone"
   - Click "Transfer ownership"
   - Enter client's GitHub username
   - Client will receive email to accept transfer

### Option 2: Fork and Pull Request
1. Client forks the repository
2. Set up GitHub Pages in the forked repository
3. Configure GitHub Actions for deployment

## Post-Transfer Maintenance

### Setting Up Collaborator Access
1. Client adds developer as collaborator:
   - Repository Settings > Collaborators
   - Click "Add people"
   - Enter developer's GitHub username
   - Select "Write" access

### Making Website Updates

#### For Small Changes (e.g., content updates, typos)
```bash
git checkout main
git pull origin main
git checkout -b fix/description-of-change
# Make changes
git add .
git commit -m "Fix: Description of changes"
git push origin fix/description-of-change
# Create pull request on GitHub
```

#### For Larger Changes
1. Create feature branch
2. Make changes
3. Create pull request with:
   - Clear description
   - Screenshots if visual changes
   - Preview link
4. Wait for client review
5. Merge after approval

## File Structure

Key directories and files:
- `_pages/` - Content pages
- `_layouts/` - Page templates
- `_includes/` - Reusable components
- `assets/` - Images, CSS, JS
- `_config.yml` - Site configuration

## Local Development

### Setup
```bash
# Install dependencies
bundle install

# Start local server
bundle exec jekyll serve --livereload
```

### Preview
- Local site: http://localhost:4000
- Changes auto-reload in browser

## Deployment

The site automatically deploys when changes are pushed to the main branch:
1. GitHub Actions builds the site
2. Deploys to GitHub Pages
3. Creates preview for pull requests

## Content Updates

### Adding New Pages
1. Create `.md` file in `_pages/` directory
2. Add front matter:
```yaml
---
layout: page
title: Page Title
permalink: /page-url/
---
```

### Adding Images
1. Add image files to `assets/images/`
2. Reference in markdown:
```markdown
![Alt text]({{site.baseurl}}/assets/images/image.jpg)
```

## Need Help?

For any questions or issues:
1. Check existing documentation
2. Create GitHub issue
3. Contact the developer through GitHub