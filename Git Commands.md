# Git Commands

### Setting Username and Email ID
- To set your username for every repository on your computer, type 
```
git config --global user.name "your_name_here"
```
- If you want to set your name for just one repository, leave out the word “global.”
- Now you can tell Git your email, make sure it’s the same email you used when you signed up for GitHub
```
	git config --global user.email "your_email@email.com"
```

### Initializing a repository
- To get started, you can create a new repository on the GitHub website or perform a `git init` to create a new repository from your project directory(local directory).
- The repository consists of three ‘trees.’ First is the *working directory*, which holds the actual files. The second one is the *index or the staging area*. Then there’s the *head*,
 which points to the last commit you made.
- If you aren’t going to create a new repository, you probably want to clone an existing repository.
- Before you can work with Git, you have to initialize a repository for your project and set it up so that Git will manage it. You can do this right on the GitHub website.

### Cloning a repository to local machine
- In order to clone a repository onto your computer, go to the repository on the GitHub website and click the big green button that says “Clone or download.”
- Make sure it says “Clone with HTTPS.” Now click the clipboard icon to copy and paste it to your clipboard
- To clone a repository, type, 
```
git clone paste-the-copied-link
```

### Checking status of the project/folder
- Use `git status` command to check the status of the files in the folder.

### Adding files to Repository
- To add files to a repository, use the command, `git add filename`
- Add all files with `git add --all` or `git add .`
	
These are your proposed changes. You can do this exact same thing with brand new files and with files that are already in there but have some changes. You aren’t actually 
adding anything just yet. You’re bringing new files and changes to Git’s attention.

### Committing the changes
- Use `git commit -m "commit message"`
- These changing are committed to the HEAD, but not to the remote repository.

### Pushing changes into repository
- To send the changes to your remote repository, run `git push` 

### Branching 
- To create a new branch, `git checkout -b branch_name`
	
### Checkout command
- Command `git checkout` lets us to check out a repository that you're not currently inside of.
- Master Branch can be checked, with the command `git checkout master`

### Merging Branches
- Branches can be merged with command `git merge branch_name`
	
### Git Pull
- To update the local repository to the newest commit, run `git pull`.

### Previewing Changes
- To preview changes before merging, run `git diff source_branch target_branch`

### Deleting Branch
- To delete a branch, run the command `git branch -d branch_name`
- The deleted branch is not available to anyone else unless pushed the branch to the remote repository with the command `git push origin branch_name`

### Untracking a file 
- To untrack a file, use `rm -rf filename` command.

### Changing Default Editor to VS Code
- To change the default code editor in git, run `git config --global core.editor "code --wait"`.

### Opening Editor 
- TO open editor from git bash, run `git config --global -e`.

## Source
[Getting started with Git and GitHub: The Complete Beginner’s Guide by Anne Bonner](https://medium.com/towards-data-science/getting-started-with-git-and-github-6fcd0f2d4ac6)

[Git Course for Beginners by Mosh](https://www.youtube.com/watch?v=8JJ101D3knE)
