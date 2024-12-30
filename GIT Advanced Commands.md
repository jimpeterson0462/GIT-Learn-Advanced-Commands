# Udemy: GIT Advanced Command
## Cognizant Yearly Elective Training
### 2024-12-29

[Udemy: GIT Advanced Command](https://cognizant.udemy.com/course/git-advanced-commands/)

#### Change the user name

	git config --global user.name "James Peterson"
	git config --global user.name jimpeterson0462@outlook.com

#### List the configuration

	git config --list

#### Edit the config in the defult editor

	git config --global -e

#### Run a difftool on a file

	git difftool [path/]filename.ext

#### Do a diff of modified files against the last commit

	git diff HEAD

#### Stage all modified files

	git add .

#### Show the status in a succinct format

	git status -s

#### Do a diff on a particular file

	git diff --cached [path/]filename.exe

#### Turn off Diff Tool Prompting

	git config --global difftool.prompt false

#### Set a global config item

	git config --global section.item value

#### View a global config item

	git config --global --get section.item

#### Set the default Diff Tool

	git config --global diff.tool diff-tool-name

#### Use a specific Diff tool

	git difftool --tool=ultracompare HEAD

#### Difference between diff and difftool

##### diff

	- Light weight built in
	- Text results in the console
	- No external apps or modules

##### difftool

	- Heavy weight external diff tool
		- such as ultracompare or winmerge etc
	- Visual interface

#### Set up an external Diff Tool

	git config --global difftool.ultracompare.cmd "\"C:\\Program Files\\ ...

#### Add a new remote repository

#### Create the repository on GitHub

- don't specify any initialization

#### Create a new local repo if you don't already have one

	git init
	git add README.md
	git commit -m "first commit"

#### Add the local repo to the remote

	git remote add origin https://github.com/mygithub/mynewrepo.git
	git push -u origin main

