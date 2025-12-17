### Introduction to Git and GitHub

- *Git*: A version control system that lets you manage and keep track of your source code history.
- *git* is version control system.popular,free &open source,fast & scalable.
- *GitHub*: A platform for hosting and collaborating on Git repositories.
- *github* allows developers to store and manage their code using git.

### Prerequisites

- Install Git on your machine: [Download Git](https://git-scm.com/downloads)
- Create a GitHub account: [GitHub](https://github.com/)

### Setting Up Git

1. *Configure Git*

   Open your terminal and set your username and email:

   bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   

### Basic Git Commands

1. *Initialize a Repository*

   Create a new directory and initialize it as a Git repository:

   bash
   mkdir my-project
   cd my-project
   git init
   

2. *Add a File*

   Create a new file:

   bash
   echo "# My Project" > README.md
   

   Add the file to the staging area:

   bash
   git add README.md
   

3. *Commit Changes*

   Commit the file to the repository:

   bash
   git commit -m "Initial commit"
   

4. *Check Status*

   Check the status of your repository:

   bash
   git status
   

5. *View Commit History*

   View the commit history:

   bash
   git log
   

### Working with GitHub

1. *Create a Repository on GitHub*

   - Go to GitHub and create a new repository named my-project.
   - Do not initialize with a README, .gitignore, or license.

2. *Connect Local Repository to GitHub*

   In your terminal, add the remote repository:

   bash
   git remote add origin https://github.com/your-username/my-project.git
   

3. *Push to GitHub*

   Push your local repository to GitHub:

   bash
   git push -u origin master
   

### Branching and Merging

1. *Create a New Branch*

   Create and switch to a new branch:

   bash
   git checkout -b new-feature
   

2. *Make Changes and Commit*

   Make some changes to a file, then add and commit:

   bash
   echo "New feature" >> README.md
   git add README.md
   git commit -m "Add new feature"
   

3. *Push the Branch to GitHub*

   Push the new branch to GitHub:

   bash
   git push origin new-feature
   

4. *Create a Pull Request*

   - Go to your repository on GitHub.
   - You’ll see a prompt to create a pull request for the new branch. Follow the steps to open a pull request.

5. *Merge the Pull Request*

   - Once the pull request is reviewed and approved, merge it into the master branch on GitHub.

6. *Update Local Repository*

   Update your local repository to reflect the changes:

   bash
   git checkout master
   git pull origin master
   

### Advanced Git Commands

1. *Stashing Changes*

   Save your uncommitted changes temporarily:

   bash
   git stash
   

   Apply stashed changes:

   bash
   git stash apply
   

2. *Undoing Changes*

   - Undo the last commit but keep the changes:

     bash
     git reset --soft HEAD~1
     

   - Undo the last commit and discard the changes:

     bash
     git reset --hard HEAD~1
     

3. *Rebasing*

   Rebase your branch onto another branch:

   bash
   git checkout new-feature
   git rebase master
   

### Example Project

Let's create a simple project to see how everything ties together:

1. *Initialize the Project*

   bash
   mkdir example-project
   cd example-project
   git init
   echo "# Example Project" > README.md
   git add README.md
   git commit -m "Initial commit"
   

2. *Create a Remote Repository*

   - Create a new repository on GitHub named example-project.

3. *Push to GitHub*

   bash
   git remote add origin https://github.com/your-username/example-project.git
   git push -u origin master
   

4. *Create a New Branch*

   bash
   git checkout -b feature-branch
   echo "This is a feature branch" > feature.txt
   git add feature.txt
   git commit -m "Add feature.txt"
   git push origin feature-branch
   

5. *Merge Feature Branch*

   - Open a pull request on GitHub for feature-branch.
   - Merge the pull request once approved.

6. *Update Local Master*

   bash
   git checkout master
   git pull origin master
   
Sure! Let's dive into the concepts of rebasing, cherry-picking, and interactive rebase.

### 1. Rebasing

*Rebasing* is a way to integrate changes from one branch into another. Instead of merging, which creates a new commit, rebasing rewrites the commit history.

#### Example: Basic Rebasing

Suppose you have a branch feature based off master, and there have been new commits on master since you started working on feature. You want to incorporate the latest changes from master into feature.

bash
# Ensure you are on the feature branch
git checkout feature

# Rebase feature branch onto master
git rebase master


This will replay the commits from the feature branch onto the master branch, effectively moving the base of feature to the tip of master.

### 2. Cherry-Picking

*Cherry-picking* is the process of picking a specific commit from one branch and applying it to another branch.

#### Example: Cherry-Picking

Suppose you have a commit in the feature branch that you want to apply to the master branch.

1. Find the commit hash you want to cherry-pick:

   bash
   git log
   

2. Cherry-pick the commit:

   bash
   git checkout master
   git cherry-pick <commit-hash>
   

This will apply the changes from the specified commit to the current branch (master in this case).

### 3. Interactive Rebase

*Interactive rebase* allows you to edit commits, squash them, reorder them, and more. It's a powerful tool for cleaning up your commit history.

#### Example: Interactive Rebase

Suppose you have several commits in your branch and you want to squash some of them together or edit commit messages.

1. Start an interactive rebase:

   bash
   git checkout feature
   git rebase -i HEAD~<number-of-commits>
   

   Replace <number-of-commits> with the number of commits you want to rebase. For example, HEAD~3 will open an interactive rebase for the last 3 commits.

2. An editor will open with a list of commits:

   
   pick f1e2d3f Commit message 1
   pick a2b3c4d Commit message 2
   pick d4e5f6g Commit message 3
   

3. You can change pick to other commands like squash (to combine commits), edit (to change commit messages), or reword (to change the commit message without editing the commit content).

   For example, to squash the last commit into the previous one:

   
   pick f1e2d3f Commit message 1
   pick a2b3c4d Commit message 2
   squash d4e5f6g Commit message 3
   

4. Save and close the editor. If you chose to squash commits, another editor window will open to allow you to combine commit messages.

### Practical Examples

#### Rebasing Example

1. *Create feature and master branches with different commits:*

   bash
   git checkout -b master
   echo "initial commit" > file.txt
   git add file.txt
   git commit -m "Initial commit on master"

   git checkout -b feature
   echo "feature commit" > feature.txt
   git add feature.txt
   git commit -m "Commit on feature branch"

   git checkout master
   echo "new master commit" >> file.txt
   git add file.txt
   git commit -m "Another commit on master"
   

2. *Rebase feature onto master:*

   bash
   git checkout feature
   git rebase master
   

#### Cherry-Picking Example

1. *Create two branches and add commits:*

   bash
   git checkout -b master
   echo "initial commit" > file.txt
   git add file.txt
   git commit -m "Initial commit on master"

   git checkout -b feature
   echo "feature commit" > feature.txt
   git add feature.txt
   git commit -m "Commit on feature branch"
   

2. *Cherry-pick the commit from feature to master:*

   bash
   git log # Get the commit hash from the feature branch
   git checkout master
   git cherry-pick <commit-hash>
   

#### Interactive Rebase Example

1. *Create a branch with multiple commits:*

   bash
   git checkout -b feature
   echo "First commit" > file1.txt
   git add file1.txt
   git commit -m "First commit"

   echo "Second commit" > file2.txt
   git add file2.txt
   git commit -m "Second commit"

   echo "Third commit" > file3.txt
   git add file3.txt
   git commit -m "Third commit"
   

2. *Start interactive rebase:*

   bash
   git rebase -i HEAD~3
   

3. *Modify the rebase instruction file:*

   
   pick f1e2d3f First commit
   squash a2b3c4d Second commit
   pick d4e5f6g Third commit
   

4. *Save and close the editor.*

5. *Edit the combined commit messages as prompted.*

### Summary

- *Rebasing*: Integrates changes from one branch into another, rewriting commit history.
- *Cherry-picking*: Applies a specific commit from one branch to another.
- *Interactive Rebase*: Allows you to edit, reorder, squash, and otherwise modify commit history.

These tools are very powerful for maintaining a clean and understandable commit history. Always be careful when rewriting history, especially on shared branches.