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

## Local Development

### Setup
```bash
# Install dependencies
bundle install

# Start local server
bundle exec jekyll serve --livereload
```