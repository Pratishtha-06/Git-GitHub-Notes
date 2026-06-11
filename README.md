# Git-GitHub-Notes

## What is Git?

Git is a free, open-source Distributed Version Control System (VCS) that you install directly onto your computer. It manages the  history of your files over time. It is a local software tool used to track changes in code. It is fast and scalable.


## What is Github?

GitHub is a cloud-based hosting platform used to share, store, manage and collaborate on those code changes.

## Commands

### Basic Commands

1. Clone & Status
- Cloning a repo on our local machine. 
```
  git clone *<repo link>*
```
- display status of code 
```
 git status
```

   Types of Status - 
   1. Untracked - new files git doesn't yet track
   2. Modified - modifying existing file
   3. Staged - files are added, ready to be commit
   4. Unmodified - unchanged files

2. Add & Commit 
- add new or changed files in your working directory to Git stagged area.
  ```
  git add *<filename>*  (specific file)
  git add .             (all files)
  ```

- commit it ... to record changes
  ```
  git commit -m "some message"
  ```

3. Push Command
- push/upload  local repo content to remote repo.

  (Can be used when branch is ahead of main/orign by any commit. Meaning local repo is ahead of remote repo).
  
  ```
   git push origin main
  ```
  ```
      git push       origin       main
     |________|     |______|     |____|
      command  cloned repo name  branch
  ```

               
