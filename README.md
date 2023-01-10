<h1>Commands of GIT for practical </h1>

## 1. Pull and Merge difference
## for pull 

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