# greenwood-library-website
Capston Project: Enhancing a community library website


## create a repo on GitHub
- repo name: greenwood-library-website

## Create a working directory for Morgan
```
mkdir morgan
cd ~/morgan/
clone git@github.com:ernynany/greenwood-library-website.git
cd greenwood-library-website
``` 

## Create the files:
- home.html
- about_us.html
- events.html
- contact_us.html

## stage and commit the files on the master branch
```
git add .
git commit -m "initial HTML structure"
git push origin master
```

## create feature branch for Morgan
```
git checkout -b add-book-reviews
``` 
**Morgan wuill add a new file boo_reviews.html**
- book_reviews.html

```
git status
git add .
git commit -m "added book reviews"
git push origin add-book-review

``` 
## create a pull request in GitHub and merge book-review --> master

## create a working directory for jamie
```
mkdir jamie
cd ~/jamie/
clone git@github.com:ernynany/greenwood-library-website.git
cd greenwood-library-website

``` 
- **also create a feature branch like in morgan's case**
```
git checkout -b update-events
``` 

## git pull to update the local maaster branch

```
cd
git pull origin master
``` 

## update the event page with new info and merge

```
git status
git add .
git commit -m "updated event page"
git push origin update-events

``` 

## merge the branch with the master
```
git checkout master
git pull origin master
git checkout add-contact-info
git merge master
```
**Note:** This will like resolve in a merge conflict since both Morgan and Jamie are working on the same index.html file. So, you have to resolve the merge conflict
- git status will show you which file the conflict is on
- manually resolve the conflict by adding or removing the wanted files.
- use vim **index.html** to edit the file

```
git status
vim index.htnl
git add index.html
git commit -m "merge conflict from add-contact-info resolved"
git push origin update-events
```

## create a pull request as jamie to add update-events --> master
- same way you created and merge Morgan's pull request to the maaster, you should also be able to create and merge Jamie's pull request to the master branch.