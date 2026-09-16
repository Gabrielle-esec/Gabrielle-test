Git mini exo (1)

Part 2: Create Your First Repository

Complete each task and write the command you used:

Create a folder called my-first-repo => mkdir my-first-repo
Navigate into that folder => cd my-first-repo
Initialize a Git repository => git init
Create a file called readme.txt => touch readme.txt then ls to check

Part 3: Your First Commit

What command shows you the current state of your repository? => git status
What command stages readme.txt for commit? => git add readme.txt
What command commits with the message "Add readme file"? => git commit -m "Add readme file"
What command shows your commit history? => git log

Part 4: Make Changes

Edit readme.txt and add a new line of text => echo "I hope im doing good." >> readme.txt
What does git status show now? Describe in your own words. the file readme.txt is modified but not staged meaning git will not include it in the next commit.
Stage and commit your changes with an appropriate message.
How many commits do you have now? I have 2 commits 

Part 5: Exploration

Try these commands and describe what they do:

git diff => It showed nothing but I searched online and it said it is suppose to show the changes made on files that have not been staged yet.
git log --oneline => Show the amount of commits with an id and their respective message
Part 6: Working with Branches

What command lists all branches in your repository? => git branch
What command creates a new branch called feature-script? => git branch feature-script
What command switches to the feature-script branch? => git switch feature-script
What single command creates and switches to a new branch called dev? => git switch -c dev
Switch back to the feature-script branch 
Verify you are on the correct branch
Part 7: Create a Bash Script on a Branch

Make sure you are on the feature-script branch

Create a new file called install.sh

Add the following content to your script:

A shebang line
A message that prints "Starting installation..."
A command to update package lists
A command to install a package of your choice
A message that prints "Installation complete!"
Make the script executable

Stage and commit your script with the message "Add install script"

Check your commit history on this branch

Part 8: Merge Branches

Switch back to the main branch

List the files in your directory. Is install.sh present? Why or why not? => install.sh does not appear because it is on the feature-script branch.

What command merges feature-script into main? => git merge feature-script

List the files again. What changed? => Now both README.txt and install.sh appear because we have merged feature-script into main

Check your commit history. What do you observe? => We have 3 commits (the one form feature-scrip was added)

What command deletes the feature-script branch after merging? => git branch -d feature-script

Part 9: Push to GitHub

Go to github.com and create a new repository called my-first-repo

⚠️ Do not initialize it with a README ⚠️

What command links your local repo to GitHub? => https://github.com/Gabrielle-esec/my-first-repo.git

What command pushes your commits to GitHub? => git push -u origin master

Refresh your GitHub page. What do you see? I see the new repo next to the first I created with the two files.

Part 10: Delete and Clone

Navigate out of your project folder

What command deletes the local repository folder? => rm -rf my-first-repo

What command clones your repository from GitHub? => git clone https://github.com/Gabrielle-esec/my-first-repo.git

Navigate into the cloned folder and verify your files are there

Part 11: Full Workflow Practice

Redo the entire exercise from scratch:

Delete your local folder
Delete the repository on GitHub
Create a new folder called bash-installer
Initialize Git
Create a README.md on main branch explaining what the project is
Commit the README
Create a branch called feature-install
On this branch get the previous installation script we've done and put it inside your current repo
Commit the script
Switch back to main
Merge feature-install into main
Delete the feature branch
Create a new GitHub repository
Push your code to GitHub
Some reflection questions

Why is version control useful?
What is the difference between staging and committing?
When should you make a commit?
What is the difference between git init and git clone?
Why should you write good commit messages?
What is the purpose of using branches?
When would you create a new branch instead of working on main?
