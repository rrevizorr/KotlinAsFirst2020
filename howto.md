Fork and clone
git remote set-url upstream https://github.com/rrevizorr/KotlinAsFirst2021(already had upstream in remotes)
git checkout -b backport
git fetch upstream
git cherry-pick d535f359...FETCH_HEAD
git remote add upstream-theirs https://github.com/Mexus209/KotlinAsFirst2021
git fetch upstream-theirs
git checkout master
git merge backport upstream-theirs/master
Fix all conflicts
git add .
git remote -v > remotes
git add *
git commit -m "foo"
git push
touch howto.md
git add *
git commit -m "howto"
git push 
