# git_cheetsheets

<!-- Git Cheetsheet -->
**What is Git ?**
 - Version Control System is a tools that helps to track changes in code.
 It is :
 - Popular
 - Free & Open Source
 - Fast & Scalable

 **What is GitHub ?**
 - GitHub is a web-based platform that uses Git for version control.
    - It provides a collaborative environment for developers to host, review, and manage code repositories.
    - It offers features like pull requests, issue tracking, and project management tools.
    - It is widely used for open-source projects and private repositories.
    - It is owned by Microsoft.

    **Basic Git Commands :**
    Initialize Repository :
    - git init : Initialize a new Git repository.

    **Clone & Status :**
    - git clone <repository_url> : Clone an existing repository from a remote source.
    - git status : Check the status of your working directory and staging area.

   ** Add & Commit :**
    - git add <file_name> : Stage changes for the next commit.
    - git commit -m "commit message" : Commit staged changes with a descriptive message.

   ** Push & Pull :**
    - git push origin <branch_name> : Push local commits to a remote repository.
    - git pull origin <branch_name> : Fetch and merge changes from a remote repository.

   ** Branching & Merging :**
    - git branch : List all branches in the repository.
    - git branch -M <new_branch_name> : Rename the current branch.
    - git checkout <branch_name> : Switch to a different branch.
    - git checkout -b <new_branch_name> : Create and switch to a new branch.
    - git branch -d <branch_name> : Delete a branch.

   **Merging :**
      Way 1 :
        - git merge <branch_name> : Merge changes from one branch into the current branch.
        - git diff : Show changes between commits, commit and working tree, etc.
        Way 2 :
         Create a Pull Request on GitHub and merge it there.

    **Other Useful Commands :**
    - git --version : Check the installed Git version.
    - git log : View the commit history.    
    - git remote add origin <repository_url> : Add a remote repository.
    - git remote -v : List all configured remote repositories.
    - git fetch : Download objects and refs from another repository.
    - git stash : Temporarily save changes that are not ready to be committed.
    - git tag <tag_name> : Create a tag for a specific commit.

   ** Undoing Changes :**

    **Case 1** : staged changes
             - git reset <file_name> : Unstage a specific file.
             - git reset : Unstage changes.
   
    **Case 2** : Commited changes (for one commit)
                - git reset HEAD~1 : Undo the last commit but keep changes in the working directory.
                
    **Case 3** : Commited changes (for multiple commits)
                - git reset HEAD~n : Undo the last n commits but keep changes in the working directory.
                - git reset <commit_id> : Undo commits up to a specific commit but keep changes in the working directory.
                - git reset --hard <commit_id> : Reset the current branch to a specific commit


   ** Rebasing & Cherry-picking :**
    - git rebase <branch_name> : Reapply commits on top of another base tip.
    - git cherry-pick <commit_id> : Apply the changes introduced by some existing commits

    ** Rename & Remove Files :**
    - git rm <file_name> : Remove a file from the working directory and staging area.
    - git mv <old_file_name> <new_file_name> : Rename or move a file.

    **Configuration Git :**
    - git config --global user.name "Your Name"   : Set the global username for Git
    - git config --global user.email "Your Email" : Set the global email for Git
    - git config --list : List all Git configurations.

    **Advanced Git Commands :**
    - git blame <file_name> : Show what revision and author last modified each line of a file.
    - git archive --format=zip --output=<file_name>.zip <branch_name> : Create a zip archive of a specific branch.

**What is GitLab ?**
 - GitLab is a web-based DevOps lifecycle tool that provides a Git repository manager.
    - It offers features like CI/CD pipelines, issue tracking, and code review.
    - It can be self-hosted or used as a cloud service (GitLab.com).
    - It is popular for both open-source and private projects.
