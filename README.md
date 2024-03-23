# Hi! This is readme-file
# This is text from branch development
mkdir new-project
cd new-project
git init
echo "# Hi! This is readme-file" > README.md
git add README.md
git commit -m "init"
git branch development
git checkout development
echo "# This is text from branch development" >> README.md
git add README.md
git commit -m "first commit from branch development: add instruction to README.md"
git checkout main
git merge development
git status
git commit -m "commit from main: merge main and development"
