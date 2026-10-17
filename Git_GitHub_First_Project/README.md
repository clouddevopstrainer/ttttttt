# My First Git & GitHub Project

A beginner-friendly project for the **Git & GitHub in 2 Hours LIVE** class.

## Project files
- `index.html` — a tiny personal profile webpage
- `style.css` — styling for the webpage
- `commands-cheatsheet.md` — important Git commands
- `.gitignore` — examples of files Git should not track

## Open the webpage
Double-click `index.html` to open it in your browser.

## Practice Git on Windows (Command Prompt)
1. Install Git from https://git-scm.com/install/windows
2. Open Command Prompt.
3. Move to the folder where you extracted this project. Example:

   ```bat
   cd %USERPROFILE%\Desktop\Git_GitHub_First_Project
   ```

4. Configure Git once (use your own name and email):

   ```bat
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git --version
   ```

5. Initialize and make your first commit:

   ```bat
   git init
   git status
   git add .
   git status
   git commit -m "Create my first project"
   git log --oneline
   ```

6. Edit `index.html`, change the introduction, then run:

   ```bat
   git status
   git diff
   git add index.html
   git commit -m "Update profile introduction"
   git log --oneline
   ```

## Publish to GitHub
1. Create and verify your account at https://github.com/signup
2. On GitHub, create a **new empty repository** named `my-first-git-project`.
   For the easiest first push, do not add a README, license, or `.gitignore` on GitHub because this folder already contains files.
3. Copy the repository HTTPS URL from GitHub. It will look like:
   `https://github.com/YOUR-USERNAME/my-first-git-project.git`
4. In Command Prompt, from this project folder, run (replace the URL):

   ```bat
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/my-first-git-project.git
   git remote -v
   git push -u origin main
   ```

GitHub may open a browser sign-in/authorization flow. Follow the prompts. Do not share your password or access token.

## Key idea
Working Directory → Staging Area → Local Repository → Remote Repository (GitHub)
