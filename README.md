# BSIT Git Practice (HTML)

A tiny multi-page site to practice Git & GitHub workflows in VS Code.

## Files
- `index.html` – home page
- `about.html` – about page (add a Team section or edit it)
- `contact.html` – contact form
- `styles.css` – minimal styling

## Suggested Git Exercises

### 0) Setup
```bash
git init
git add .
git commit -m "chore: initial commit with 3 HTML pages and CSS"
```

### 1) Branching & commits
```bash
git checkout -b feature/add-blog
# Create blog.html and link it in the nav of all pages
git add blog.html index.html about.html contact.html
git commit -m "feat: add blog page and update navigation"
```

### 2) History & diffs
```bash
git log --oneline --graph --decorate
git diff HEAD~1
```

### 3) Merge
```bash
git checkout main
git merge feature/add-blog
```

### 4) Remote (GitHub)
```bash
git remote add origin https://github.com/<username>/<repo>.git
git branch -M main
git push -u origin main
```

### 5) Pull request & conflicts
- On GitHub, open a PR from a new branch (e.g., `feature/change-button-text`).
- Have another student edit the same line differently on another branch.
- Pull both locally and resolve the conflict in VS Code, then commit & push.

Happy practicing!
