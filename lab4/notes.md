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
