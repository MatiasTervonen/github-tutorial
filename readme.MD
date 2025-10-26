# GitHub Tutorial

How to get started

1. Install Git

Install Git on your computer.
You can also install GitHub Desktop, which provides a graphical interface to make it easier to manage Git repositories.
GitHub Desktop includes Git automatically.

2. Configure Your Profile

Before you start using Git, configure your username and email:

git config --global user.name "Your Name Here"
git config --global user.email "your@email.com"

3. Initialize Repository

To start tracking a project with Git.

git init

4. Add Files to the Repository

add all files

git add .

add a specific file

git add <folder name>

4. To see which branch you’re currently on and what changes have been made:

git status

5. Create a new branch

git branch <branch name here>

See all branches and which one you’re currently on

git branch

Switch to another branch

git checkout <branch name> / git switch <branch name>

6. Commit changes

git commit -m "commit name here"

7. Push commits to the github

git push -u origin <branch name>


When working in a team on GitHub, you almost always work on a branch.
If you starting to implement a new feature, create a new branch for it.
This keeps your changes separate until they are reviewed and ready to merge into the main branch.

If you are working solo, you can work directly on the main branch and push your changes there

Clone the repository. Make a new feature/branch and push your changes there.

Example workflow

1. Clone repository

git clone https://github.com/MatiasTervonen/Training-App.git
cd training-app

2. Make a new feature branch

git checkout -b feature/login

3. Make your changes then add and commit them 

git add .
git commit -m "Add login page"

4. Push your changes to github

git push -u origin feature/login

5. Make a pull request
 
- Go to the repository on GitHub. You see Compare & pull request button - clik it. 
Add title and description explaining your changes. When you are ready click "create pull request". 
Your team will review the changes, and if there is no issues, the pull request will be merged to the main branch.