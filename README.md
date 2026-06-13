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

               
4. Init Command
- to initialize repo/ create new repo

```
  git init                                (initialize)
  git remote add origin *<repo-link>*     (add remote repo to our local machine)
  git remote -v                           (to verify repo) 
  git branch                              (to check branch) 
  git branch -M *<name>*                  (rename branch) 
```

### Work Flow 
```
    Create Git Repo
          |
      Clone repo
          |
     make changes
          |
     add changes
          |
    commit changes
          |
     push changes
           
```

## Git Branches 

*Branch Diagram*
                                        
                        __|branch 1|-----|  (merge point)
                       |                 | / 
--------|main branch|------------(MB)----|------- main branch(merge all branches)
                       |__               |
                          |branch 2|-----| 

### Branch Commands

1. git branch - to check branch
2. git branch -M main - to rename branch
3. git checkout *<branch-name>* - to navigate
4. git checkout -b *<new-branch-name>* - to create new branch
5. git checkout -d *<branch-name>* - to delete branch

### Merge Comands

*Way 1 -*

- to compare commits, branch files and more
```
 git diff <branch-name>
```

- to merge branches
```
 git merge <branch-name>
```

*Way 2 -*

- Create PR(pull request) on github

Pull Request - It lets you tell others about the changes you've pushed to a branch in a repository on Github.