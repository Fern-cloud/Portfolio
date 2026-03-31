# Portfolio
A portfolio website for Fern Lewis, written in HTML, CSS, and JS.

# How to edit:
Quick 6‑step workflow — edit locally, commit, and publish (recommended)
1. Open your project folder in your code editor (VS Code, Sublime, etc.).  
2. Edit files (index.html, style.css, script.js, responsive.css). Save changes.  
3. In terminal, confirm branch and status:
   ```
   git branch --show-current
   git status
   ```
4. Stage and commit your changes:
   ```
   git add .
   git commit -m "Update: <short description of change>"
   ```
5. Pull remote changes first (avoid being behind) and rebase:
   ```
   git pull --rebase origin main
   ```
   Resolve any conflicts (edit files, git add <file>, git rebase --continue).  
6. Push your update:
   ```
   git push origin main
   ```
   Your GitHub Pages site will update automatically within a minute or two.

### Quick alternative — edit via GitHub web (fast for small content tweaks)
1. Open the file in your repo on github.com.  
2. Click the pencil (Edit) icon, make changes in the web editor.  
3. Add a short commit message and choose “Commit directly to the main branch” (or create a branch + PR if preferred).  
4. Save; the site will update shortly.

### Tips & troubleshooting
- Preview locally by opening index.html in your browser or use Live Server in VS Code for hot reload.  
- If site doesn’t reflect changes, clear browser cache (Ctrl/Cmd+Shift+R) or use a private window.  
- To undo a bad commit:
  - If not pushed: `git reset --hard HEAD~1`
  - If pushed: create a revert commit: `git revert <commit-hash>`  
- For larger changes, create a feature branch:
  ```
  git checkout -b feature/my-change
  # make changes, commit, push
  git push -u origin feature/my-change
  ```
  Then open a Pull Request on GitHub to merge.

Teacher Tip: treat each saved commit like a snapshot — write clear commit messages so you can trace changes easily.

Analogy: editing your site is like updating a printed flyer — you change the master file, save a new version, and send it to the printer (GitHub Pages) to publish.

Which method would you like step‑by‑step help with now (local edits with Git, or GitHub web edits)?
