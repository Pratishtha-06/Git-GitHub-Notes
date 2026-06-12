# Git-GitHub-Notes

### What is Git?

Git is a free, open-source Distributed Version Control System (VCS) that you install directly onto your computer. It manages the  history of your files over time. It is a local software tool used to track changes in code. It is fast and scalable.

## What is Github?

GitHub is a cloud-based hosting platform used to share, store, manage and collaborate on those code changes.

Remote repo - Github repo
Local repo - on our local machine


## Commands

### Basic Commands

1. Clone & Status
- Cloning a repo on our local machine. 
  command -> git clone *<repo-link>*

- display status of code 
  command -> git status

 Types of Status - 
 1. Untracked - new files git doesn't yet track
 2. Modified - modifying existing file
 3. Staged - files are added, ready to be commit
 4. Unmodified - unchanged files
  
  
2. Add & Commit 
- add new or changed files in your working directory to Git stagged area.
  command -> git add *<filename>* (specific file)
  command -> git add . (all files)

- commit it ... to record changes
  command -> git commit -m "some message"

3. Push Command
- push/upload  local repo content to remote repo
  command -> git push origin main
  (Can be used when branch is ahead of main/orign by any commit. Meaning local repo is ahead of remote repo)
      git push       origin       main
     |________|     |______|     |____|
      command  cloned repo name  branch


4. Init Command
- to initialize repo/ create new repo


-> git init                                (initialize)
-> git remote add origin *<repo-link>*     (add remote repo to our local machine)
-> git remote -v                           (to verify repo) 
-> git branch                              (to check branch) 
-> git branch -M *<name>*                  (rename branch) 