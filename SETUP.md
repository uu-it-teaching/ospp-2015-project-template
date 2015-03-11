# Clone your empty project repository

```bash
$> git clone https://github.com/uu-it-teaching/ospp-2015-group-xx.git
Cloning into 'ospp-2015-group-xx'...
warning: You appear to have cloned an empty repository.
Checking connectivity... done.
$>
```

```bash
$> cd ospp-2015-group-xx
```

## Add the remote template repository

```bash 
$> git remote add template https://github.com/uu-it-teaching/ospp-2015-project-template.git
```

Check all remote repositories. 
```bash
$> git remote -v
origin	https://github.com/uu-it-teaching/ospp-2015-group-xx.git (fetch)
origin	https://github.com/uu-it-teaching/ospp-2015-group-xx.git (push)
template	https://github.com/uu-it-teaching/ospp-2015-project-template.git (fetch)
template	https://github.com/uu-it-teaching/ospp-2015-project-template.git (push)
$>
```

## Fetch the template 
Now fetch the content of the template repository. 

```shell
$> 11:46:26 > git fetch template
remote: Counting objects: 177, done.
remote: Compressing objects: 100% (154/154), done.
remote: Total 177 (delta 67), reused 8 (delta 2), pack-reused 0
Receiving objects: 100% (177/177), 56.45 KiB | 0 bytes/s, done.
Resolving deltas: 100% (67/67), done.
From https://github.com/uu-it-teaching/ospp-2015-project-template
 * [new branch]      master     -> template/master
$>
```
## Merge

```shell
$> git merge template/master
```
## Remove the template remote repository
```shell
$> git remote remove template
```

Check ...

```shell
$> git remote -v
origin	https://github.com/uu-it-teaching/ospp-2015-group-xx.git (fetch)
origin	https://github.com/uu-it-teaching/ospp-2015-group-xx.git (push)
$> 
```
## Push

```shell
$> git push --all
Counting objects: 177, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (89/89), done.
Writing objects: 100% (177/177), 56.45 KiB | 0 bytes/s, done.
Total 177 (delta 67), reused 177 (delta 67)
To https://github.com/uu-it-teaching/ospp-2015-group-xx.git
 * [new branch]      master -> master
$>
```
