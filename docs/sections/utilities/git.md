icon: simple/git

#![AWS CLI Banner!](/assets/01-header-images/git.png "Image of AWS CLI")

## Delete all local branches except main/master
```
git branch | grep -v "main" | xargs git branch -D
```
!!! Tip
    Replace main with branch of your choice