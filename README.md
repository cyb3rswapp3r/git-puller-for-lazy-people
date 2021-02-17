<p align="center">
    •<a href="git-puller-for-lazy-people">Overview</a>•
    <a href="usage">Usage</a>•
    <a href="soon">Coming Soon</a>•
</p>

# Git-Puller-For-Lazy-People

This is just a shell script I use to do git pull on all the cloned repositories that I have. It's a pretty lazy idea but I just like to automate the simple things.

# Usage

First you need to clone the repository into your machine:
```bash
$ git clone https://github.com/i-am-jezz/git-puller-for-lazy-people.git
$ cd git-puller-for-lazy-people/
$ chmod +x git_pull_script
$ ./git_pull_script git_repos.txt
```

To create the file containing path to git repositories:
```bash
$ find / -name .git 2>/dev/null | tee git_repos.txt
```
This command will create the file <i>git_repos.txt</i> which contains the path to all the github repositories in your system. If you don't want to pull a specific repository remove it's path from the git_folders.txt file. 

<b>NOTE</b>:The git_repos.txt file will contain the path to the files with <i>.git</i> at the end. You will need to remove the extension. This can be done easily by doing a find & replace on the text file.

# Soon

I'm working on a script to load the the git_repos.txt file automatically.
