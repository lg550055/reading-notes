# Git intro

### Git is a distributed version control system that enhances collaboration

- Git stores data in a file system made of snapshots
- Git mostly relys on local operations -most necessary information can be found in local resources
- Git tracks changes to files or directories

#### Git basics

Your system probably already has git installed; if not download it and install it

##### Create a repository and commit changes
1. Navigate to your project directory (`cd [path]`)
2. Initialize you repository: `git init`
3. Add files to track: `git add [filename]` or `git add .` to add all files
4. Input `git commit -m "commit message"` to record your changes

#### Clone a repository (i.e. copy a repository form a server)
Use `git clone [url]` usually this url is a github account

#### Other basic commands
- To determine the state of files, use `git status`
- Use `git push origin main` to upload your changes to a remote repository

*That's all for now!*


*[Back to home page](index.md)*
