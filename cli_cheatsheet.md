1) Git Commands
git add . => Puts all changed files into the staging area.
git commit -m "message" => Saves the staged changes as a commit.
git log => Shows the full commit history.
git log --oneline => Shows commit history in a short form.
git log --oneline --graph --all => Shows commits and branches in a graph.
git show => Shows the details of a commit and what was changed.
git diff => Shows changes that are not staged.
git diff --staged => Shows changes that are already staged.
git checkout -b branch-name => Creates a new branch and moves to it.
git branch => Shows all branches. * means current branch.
git switch branch-name => Moves to another branch.
git switch -c branch-name => Creates a new branch and moves to it.
git switch main => Moves to the main branch.
git merge experiment => Brings the changes from experiment into your current branch.
git merge --abort => Cancels a merge that has a conflict.
git branch -d experiment => Deletes the experiment branch.
git push => Sends your commits from your computer to GitHub.
git remote -v => Shows the GitHub repository connected to your project.




2) Terminal Commands
cd folder-name => Goes inside a folder.
cd .. => Goes one folder back.
pwd => Shows where you are.
ls => Shows files and folders.
dir => Also shows files and folders.


3) Searching Files
Get-ChildItem -Recurse -Filter *.py => Finds all Python files in the current folder and its subfolders.
Get-ChildItem -Recurse -Filter *.py | Select-String "def " => Finds where functions (def) are written in Python files.
Get-ChildItem -Recurse -File | Select-String "print" | Measure-Object => Counts how many lines contain print.
(Get-ChildItem -Recurse -Filter *.py).Count => Counts the total number of Python files.


4) Working With Files
dir > contents.txt => Saves the output of dir into contents.txt.
Get-Content contents.txt => Shows what's written inside contents.txt.



5) Merge Conflict
Step-1 => git switch main : Go To Main
Step-2 => git merge feature : Merge Feature into Main
Step-3 => git status : Check Wich File has in conflict
Step-4 => open the conflict file
Step-5 => choose a code which you want to keep
Step-6 => git add .
Step-7 => git commit -m "merge conflict"
Step-8 => git status
Step-9 => git log --oneline --graph --all
