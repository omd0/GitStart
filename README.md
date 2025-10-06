# Hello World Git Repository

A simple web page demonstrating basic HTML, CSS, and Git usage.

## 🚀 Getting Started

This repository contains a basic "Hello World" web page built with:

- **HTML5** - Semantic markup structure
- **CSS3** - Modern styling with gradients and responsive design
- **Git** - Version control for tracking changes

## 📁 Project Structure

```
GitStart/
├── index.html          # Main HTML file
└── README.md          # This file
```

## 🌐 Viewing the Page

Simply open `index.html` in your web browser to see the Hello World page.

## 🛠️ Features

- Responsive design that works on desktop and mobile
- Modern gradient background
- Clean, professional styling
- Git repository information display

## 📝 Git Setup & Commands

### First Time Git Setup

Before using Git, configure your identity:

```bash
# Set your name (replace "Your Name" with your actual name)
git config --global user.name "Your Name"

# Set your email (replace with your actual email)
git config --global user.email "your_email@example.com"

# Verify your configuration
git config --list
```

### Repository Commands

To get started with this repository:

```bash
# Initialize the repository (if not already done)
git init

# Add files to staging
git add .

# Make your first commit
git commit -m "Initial commit: Add Hello World web page"

# Check status
git status
```

### Forking and Pushing to Remote

To share your repository on GitHub:

1. **Fork the repository on GitHub:**
   - Go to the original repository on GitHub
   - Click the "Fork" button in the top-right corner
   - This creates a copy in your GitHub account

2. **Add remote origin:**
   ```bash
   # Add your forked repository as remote origin
   git remote add origin https://github.com/YOUR_USERNAME/GitStart.git
   
   # Verify remote was added
   git remote -v
   ```

3. **Push to GitHub:**
   ```bash
   # Push your commits to GitHub (first time)
   git push -u origin master
   
   # For subsequent pushes
   git push
   ```

4. **Pull updates (if working with others):**
   ```bash
   # Pull latest changes from remote
   git pull origin master
   
   # Alternative: Pull and rebase (cleaner history)
   git pull --rebase origin master
   
   # Pull from a specific branch
   git pull origin main
   
   # Pull all branches from remote
   git fetch --all
   git pull --all
   ```

5. **Advanced Pull Commands:**
   ```bash
   # Check what changes will be pulled (without actually pulling)
   git fetch origin
   git log HEAD..origin/master --oneline
   
   # Pull with verbose output to see what's happening
   git pull -v origin master
   
   # Pull and automatically resolve conflicts with local changes
   git pull --strategy=recursive -X theirs origin master
   
   # Reset to match remote exactly (WARNING: loses local changes)
   git fetch origin
   git reset --hard origin/master
   ```

6. **Handling Merge Conflicts:**
   ```bash
   # If conflicts occur during pull
   git status                    # See conflicted files
   # Edit files to resolve conflicts
   git add .                     # Stage resolved files
   git commit                    # Complete the merge
   
   # Abort the pull if you want to start over
   git merge --abort
   ```

## 🎯 Purpose

This project serves as a learning tool for:
- Basic web development (HTML/CSS)
- Git version control
- Repository management
- Web page deployment

## 📄 License

This project is open source and available under the MIT License.
