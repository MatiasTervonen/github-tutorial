# GitHub Tutorial

**How to get started**

1. Install Git

Install Git on your computer.
You can also install GitHub Desktop, which provides a graphical interface to make it easier to manage Git repositories.
GitHub Desktop includes Git automatically.

[Git](https://git-scm.com/)  
[GitHub Desktop](https://desktop.github.com/download/)

2. Configure Your Profile

Before you start using Git, configure your username and email:

```bash
git config --global user.name "Your Name Here"
git config --global user.email "your@email.com"
```

3. Initialize Repository

To start tracking a project with Git.

```bash
git init
```

4. Add Files to the Repository

Add all files

```bash
git add .
```

Add a specific file

```bash
git add <folder name>
```

4. To see which branch you’re currently on and what changes have been made:

```bash
git status
```

5. Create a new branch

```bash
git branch <branch name here>
```

See all branches and which one you’re currently on

```bash
git branch
```

Switch to another branch

```bash
git checkout <branch name>
```

6. Commit changes

```bash
git commit -m "commit name here"
```

7. Push commits to the github

```bash
git push -u origin <branch name>
```

When working in a team on GitHub, you almost always work on a branch.
If you starting to implement a new feature, create a new branch for it.
This keeps your changes separate until they are reviewed and ready to merge into the main branch.

If you are working solo, you can work directly on the main branch and push your changes there

Clone the repository. Make a new feature/branch and push your changes there.

**Example workflow**

1. Clone repository

```bash
git clone https://github.com/MatiasTervonen/Training-App.git
cd training-app
```

2. Make a new feature branch

```bash
git checkout -b feature/login
```

3. Make your changes then add and commit them

```bash
git add .
git commit -m "Add login page"
```

4. Push your changes to github

```bash
git push -u origin feature/login
```

5. Make a pull request

- Go to the repository on GitHub. You see Compare & pull request button - clik it.
  Add title and description explaining your changes. When you are ready click "create pull request".
  Your team will review the changes, and if there is no issues, the pull request will be merged to the main branch.

**Version control**

1. See all past changes, shows all past commits wih unique commit ID.

```bash
git log
```

Quit log

```bash
q
```

2. Go back to pervious version. You can look old version without changin hiostory.

```bash
git checkout <commit-id>
```

3. Revert specific commit (Safe Way). If you made a mistake and want to undo it without deleting history.
   It keeps the old commit in hiostory and creates new commit that reverses it.

```bash
git revert <commit-id>
```

4. Hard reset. Go to back permanently. (Dangerous)
   Moves project back to specific commit and deletes all commits that came after it.

```bash
git reset --hard <commit-id>
```
