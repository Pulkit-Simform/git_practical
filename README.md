<h1>Commands of GIT for practical </h1>



<!-- TOC -->

- [Practical Test](#index)
    - [1. Pull and Merge difference](##1-Pull-and-Merge-difference)
    - [2. Rebase](##2-Rebase)
    - [3. Change Commit Message](##3-Change-Commit-Message)
    - [4. Cherry Pick](##4-Cherry-Pick)
    - [5. Drop commit](##5-Drop-commit)
    

<!-- /TOC -->


## 1. Pull and Merge difference
### for pull 

```bash
    git pull
```
### pull screenshot

<img src="images/pull_1.png" title="pull from github"/>
<br/>
<img src="images/pull_2.png" title="pull from github to local"/>


### for merge 
```bash
    git merge <branch-name>
```
<img src="images/git_merge.png" title="git merge from feature branch to master" />

<br />

## 2. Rebase

```bash
    git rebase <branch-name>
```
<img src="images/git_rebase.png" title="git rebase from feature branch to master" />



## 3. Change Commit Message

```bash
    git rebase -i @~n    # here n stands for to the n commit that we want to change
    # and inside we have to use reword
    # or if we want to change last then we have to use
    git commit --amend

    # here we have used git commit --amend for rewording last commit
```
<h3>Before renaming check de2da56 </h3>
<img src="images/git_rename_before.png" title="git rename before" />

<h3>After renaming check de2da56 </h3>
<img src="images/git_rename_after.png" title="git rename before" />

## 4. Cherry Pick


```bash
   git cherry-pick <hash-code-of commit>

   e.g. git cherry-pick df88675
```


<h3>Before cherry-pick  </h3>
<img src="images/git_cherry_pick_before.png" title="git cherry-pick before" />

<h3>After cherry-pick  </h3>
<img src="images/git_cherry_pick_after.png" title="git cherry-pick after" />



## 5. Drop commit


```bash
   git rebase -i @~n # n from where to pick

   # and then inside choose the commit name
   # after choosing commit name use "drop" for dropping the commit


   !# and for last change simply used
   git reset HEAD^ # and then commit it

```

<h3>Git log  for dropping 98ca8ce</h3>
<img src="images/git_drop_1.png" title="git log drop for " />

<h3>adding drop inside git rebase</h3>
<img src="images/git_drop_2.png" title="edit inside git rebase and add drop option" />

<h3>Successfully dropped commit 98ca8ce</h3>
<img src="images/git_drop_3.png" title="dropped commits" />

<h3>Git log after dropped</h3>
<img src="images/git_drop_4.png" title="git log after dropped " />



