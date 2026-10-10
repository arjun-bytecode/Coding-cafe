Question 1:The --global flag means this configuration applies to all Git repositories for your user account on this computer. If you left it out, the configuration would only apply locally to the current repository you are in.

Question 2:The .git directory appeared in ls -a(.  ..  .git  .venv  README.md  week01  week02) but not in ls(README.md  week01  week02) because it is a hidden folder. It contains all the internal tracking data, history, and configuration that Git uses to manage this specific repository.

Question 3:
Git offered to track a few items in the directory, such as README.md, week01, and week02. If a .venv/ folder was populated, it would try to track hundreds of files of virtual environment code that I did not write. 
output:On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        week02/

nothing added to commit but untracked files present (use "git add" to track)

Question 4:The files and folders specified in the .gitignore file (such as .venv/, __pycache__/, *.pyc, and .DS_Store) disappeared from the untracked files list. Git is now ignoring them.
Output:On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        README.md
        week02/

nothing added to commit but untracked files present (use "git add" to track)

Question 5:The .gitignore file should be committed, not ignored. It needs to be tracked by Git so that anyone else working on the repository will have the exact same rules for ignoring files.

Question 6:It moved from "Untracked files" to "Changes to be committed". In the three-places model, the file was moved from the Working Directory into the Staging Area.

Question 7:Git printed the branch name, the short commit hash, and the commit message ("Lab work so far"). It also printed a summary of exactly how many files were changed and how many lines were inserted.
Output:
[master (root-commit) 50d23ee] Lab work so far
 4 files changed, 98 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 week02/lab01-log.txt
 create mode 100644 week02/notes.md

Question 8:The first seven characters are called the short commit hash (or SHA-1 hash). They serve as a unique identifier for that specific commit, allowing you to reference it in the project's history.
Output:50d23ee

Question 9:The four steps of the loop are editing or creating a file, checking the repository's state with git status, moving the changes to the staging area with git add, and saving them to the history with git commit. Running git log is often done afterward to verify the new commit was added to the timeline.

Question 10: README.md is a universal convention across software development and platforms like GitHub. GitHub automatically parses and displays the contents of README.md on the front page of the repository, serving as the landing page and overview for anyone viewing the project.

Question 11:
The gh auth login command authenticated your terminal with GitHub using a secure web token instead of a traditional password. By selecting "Yes (authenticate Git)" during the setup, it configured Git to use the GitHub CLI as a credential helper, which automatically provides this stored token in the background whenever you push.

Question 12:
The front page now displays the rendered contents of your README.md file. GitHub is designed to automatically detect and display the README file at the root of a repository so visitors immediately see the project's overview and instructions.

Question 13:
No, pushing does not change your local commit history. It simply copies your local commits to the remote repository on GitHub and updates your local Git's awareness of where the remote branch (origin/main) currently sits.

Question 14:
A private repository exists on GitHub's servers and is accessible to you and any specific users you explicitly invite as collaborators, such as your TAs. If a repository does not exist on GitHub at all, it only lives locally on your computer's hard drive and cannot be viewed, shared, or backed up online.
