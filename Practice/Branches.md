
### Creating branches with `git branch`

```bash
#syntax
git branch <branch_name> 

#example
git branch feature1 #this will create a branch named 'feature1'

#If you wish to see the branches that are available
git branch
```

![](https://i.imgur.com/wfxdrK2.png)

### Creating branches with `git checkout`

```bash
# this will create new branch and also checkout to that branch
git checkout -b <branch_name> 

#example
git checkout -b feature2 #this will create a branch named 'feature1'

#If you wish to see the branches that are available
git branch
```

### `git init` initialise new repository 
```bash
#Creating a new repo
git init website-flow

#Creating some dummy files and commiting them
cd website-flow

echo "<h1>This is my website</h1>" > index.html

# git add is used track file changes
git add index.html

# git commit is used to commit changes permanently
git commit -m "Created index.html"
echo "h1, h2, h3 { margin-bottom: 15px; }" > style.css
git add style.css
git commit -m "Created style.css"

#Checking out the logs
git log --all --graph
```

![](https://i.imgur.com/uYNe7vq.png)

```bash
# this will list down all branches
git branch
  
#creating file new files
echo "feature 0.1" > new_edition.html

git add new_edition.html

git commit -m "added a new feature 0.1"
 

echo "feature 0.2" >> new_edition.html

git add new_edition.html

git commit -m "modified new_edition.html and added new functionality, feature 0.2"
  
#Checking out the logs
git log --all --graph  

```
![](https://i.imgur.com/FbI2L6h.png)

```bash
# switching to specified branch 
git checkout feature1
ls

#to see the files in the main branch
git checkout main
ls
```
![](https://i.imgur.com/dzaDtzS.png)

```bash
#ensuring we are in the main branch
git branch

#making a hotfix in the main branch
echo "hotfix 1.0" >> hotfix.txt

git add hotfix.txt
git commit -m "fixed a bug"

#Checking out the logs
git log --all --graph
```
![](https://i.imgur.com/x1IEQAh.png)

```bash
#switching to feature1 branch
git checkout feature1

#checking out the files here
ls

#Checking out the logs
git log --all --graph
```

![](https://i.imgur.com/wHMPibb.png)


```bash
#adding repo remote to git
git remote add origin https://github.com/kailashinventyv2024/test.git

#switching to main branch
git checkout main

#pushing the main branch
git push origin main

#performing fetch
git fetch

#trying again but forced update this time
git push origin main -f

```

```bash
#pushing the feature1 branch
git push origin feature1
```

![](https://i.imgur.com/Oqa65P6.png)


```bash
#ensuring we are in the main branch
git checkout main

#merging two branches
git merge feature1 -m "merging feature1 back to main"

#checking the files now
ls
```

![](https://i.imgur.com/JALyG9m.png)


```bash
#Checking out the logs 
git log --all --graph
```

![](https://i.imgur.com/BZzvyPB.png)

### Merge Conflicts
##### Creating a merge conflict

![](https://i.imgur.com/lbcgMs2.png)

### Trying to merge branch with conflict 
![](https://i.imgur.com/5Rfl8aD.png)


![](https://i.imgur.com/7rAJrvW.png)

### List down file content
![](https://i.imgur.com/SlRiJwG.png)

### After  resolving conflict
![](https://i.imgur.com/k9pPuVF.png)

### Practice branching and commands

![](https://i.imgur.com/IkmwilI.png)

![](https://i.imgur.com/xlktCP8.png)
