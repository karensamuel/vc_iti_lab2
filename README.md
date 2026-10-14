git init\
git commit -m "first commit"\
git branch -M main\
git remote add origin git@github.com:karensamuel/vc_iti_lab2.git \
git push -u origin main \
-- add txt file for commands \
git add . \                  
 git commit -m "added txt files"
 // create dev branch  and add the new file 
 git branch dev
 git switch dev
 git add .                     
 git commit -m "added dev files"
 git push  origin dev
  // create test branch  and add the new file 

git branch test
git checkout test
git add .
git commit -m "added test file"
git push origin test
// merge the dev with test
 git checkout dev
git merge test
git add .                     
 git commit -m "merge  test done"
 // merge dev to main
  git checkout main
git merge dev
git add .                     
 git commit -m "merge  dev done"
// Tell me how to remove them locally and remotely.
remotely:
git push origin :test  
git push origin :dev  
locally:
git branch -d test
git branch -d dev
// Tell me how to checkout another branch without commit
changes
git stash
git stash pop

//Create an annotated tag with tagname (v1.7) .
 git tag -a v1.0 -m "version1.0"
● Push it to the remote repository.
git push origin v1.0
● Tell me how to list tags.
 git tag 
● Tell me how to delete tag locally and remotely.
remotely:
 git push origin --delete v1.0
 locally:
 git tag -d v1.0
● Add an image in the README.md file.
![iti logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR96y7zflaG7F5vdA3iSPkhXo8mUroISA0Lj9bTt2c7hKeOKJKOCM5LyAA&s=10)
git add .
git commit -m "added image"
git push 