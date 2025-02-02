# Git Commands Tutorial for DevOps

## Setting Up a Git Repository
Git allows you to initialize a new repository where you can track changes to files.
```sh
mkdir git-for-devops   # Create a new directory
cd git-for-devops/     # Move into the directory
pwd                    # Print working directory
git init               # Initialize an empty Git repository
ls -a                  # List all files including hidden ones
```

## File Operations
Git works with files, and you can create, modify, and delete them.
```sh
vim hello-dosto.txt   # Create and edit a file
ls -l                 # List files with details
rm hello-dosto.txt    # Remove a file
vim hello-dosto.txt   # Recreate the file
ls -l                 # Check file again
clear                 # Clear the terminal screen
```

## Checking Git Status
You can check the status of your repository to see which files have changed.
```sh
git status              # Check the status of your repository
touch hello.txt         # Create a new file
ls                      # List files
touch nibba.txt nibbi.txt  # Create multiple files
git status              # See the new untracked files
rm hello.txt            # Remove a file
git status              # Check the status again
```

## Staging and Unstaging Files
Before committing, you must add files to the staging area.
```sh
git add nibbi.txt      # Stage a single file
git status             # Check status
git add nibba.txt      # Stage another file
git status             # Check status
git rm --cached nibba.txt  # Unstage a file
git status             # Verify status
git add nibba.txt      # Re-add the file
git status             # Check status again
```

## Committing Changes
After staging, you can commit the changes to save a snapshot.
```sh
git commit -m "adding nibba nibbi"  # Commit changes with a message
ls
rm nibbi.txt    # Remove a file
ls
git status      # Check status
git restore nibba.txt  # Restore the deleted file
ls
git restore nibbi.txt  # Restore another deleted file
ls
```

## Configuring Git User
Git requires a username and email to track commits properly.
```sh
git config --global user.name "awstest264"   # Set username
git config --global user.email "awstest264@gmail.com"  # Set email
```

## Modifying and Committing Changes
You can modify a file and commit it again.
```sh
vim nibbi.txt   # Edit the file
git status      # Check status
git add nibbi.txt   # Stage changes
git commit -m "added new changes to nibbi"  # Commit with a message
git status      # Verify status
clear          # Clear terminal
```

## Additional Commits and Restoring Files
```sh
git init             # Initialize a repository
vim friend.txt       # Create and edit a file
git add friend.txt   # Stage the file
git status          # Check status
git commit -m "new added"  # Commit file
git status          # Verify status
ls
rm friend.txt       # Remove the file
ls
git status          # Check repository status
git restore friend.txt   # Restore the removed file
ls
```

## Viewing Git History
You can view previous commits using the log command.
```sh
git log          # Show commit history
clear           # Clear the screen
git log --oneline  # Show a summarized history
```

## Working with Branches
Branches allow you to work on different features independently.
```sh
git branch            # List all branches
git checkout -b dev   # Create and switch to a new branch
git branch            # Verify branches
```

## Switching Branches and Merging Changes
```sh
vim nibbu.txt     # Create and edit a file
git status        # Check changes
git add nibbu.txt # Stage changes
git commit -m "new nibbu added"  # Commit new file
git status        # Check repository status
git checkout master   # Switch back to master branch
git status        # Check status
ls               # List files
git checkout dev # Switch back to dev branch
git log          # View log
git branch       # Verify branches
git checkout master   # Switch to master branch
clear            # Clear screen
```

## Checking Logs in Short Format
```sh
git log --oneline  # View compact log
git checkout dev   # Switch to dev branch
git log --oneline  # View log in dev branch
```

This tutorial covers basic Git operations useful for DevOps. Let me know if you need more details! 🚀
