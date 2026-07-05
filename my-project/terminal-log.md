Task 5.1 – Terminal Navigation

pwd
ls
cd ~
pwd
cd /workspaces
ls
cd /workspaces/iyf-s11-week-03-Mkmoise
pwd

Task 5.2 – File Operations

Exercise 1

touch index.html
cat index.html
cp index.html backup.html
mv backup.html docs/
mv index.html home.html
rm home.html

Exercise 2

mkdir -p my-project/src/css
mkdir -p my-project/src/js
mkdir -p my-project/src/images
mkdir my-project/docs
mkdir my-project/tests
touch my-project/src/index.html
touch my-project/src/css/styles.css
touch my-project/src/js/main.js

cp -r my-project/src my-project/src-backup
mkdir my-project/archive
mv my-project/src-backup my-project/archive/
ls my-project/archive
rm -r my-project/archive
ls my-project

Task 5.3 – Useful Terminal Commands

find . -name "*.html"
find . -name "*.css"
find . -name "*.js"

grep "class" my-project/src/index.html
grep -r "button" my-project

history
history | tail -10

head -10 my-project/README.md
tail -10 my-project/README.md

wc my-project/README.md
wc -l my-project/README.md

find . -name "*.html" | wc -l
grep -r "contact" .
wc -l my-project/src/css/styles.css
history | tail -10

## Task 5.4 – Shell Script Basics

touch new-project.sh
code new-project.sh
chmod +x new-project.sh
./new-project.sh my-awesome-app
ls my-awesome-app
ls -R my-awesome-app

Task 6.1 – Git Basics
git config --list
git status
git log --oneline

## Task 6.2 – Branching & Merging

git branch
git branch feature/contact-form
git checkout feature/contact-form
echo "## Contact Form Feature Branch" >> README.md
tail -5 README.md
git add README.md
git commit -m "feat: update README on contact feature branch"
git checkout main
git merge feature/contact-form
git branch -d feature/contact-form
git push

## Task 6.3 – GitHub Remote Workflow

git remote -v
git push
git status
cd /workspaces
git clone https://github.com/musembijoel/iyf-s11-week-03-musembijoel.git week03-clone
ls
cd /workspaces/iyf-s11-week-03-musembijoel
touch .gitignore
git add .
git commit -m "feat: add .gitignore"
git push
