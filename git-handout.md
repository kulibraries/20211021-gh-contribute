# Introduction to Git and GitHub Workshop Handout

## ArchivesSpace Kansas City Regional Forum
## November 30, 2018

---

Personnel:
- Jamene Brooks-Kieffer, KU Libraries
- Tami Albin, KU Libraries
- Scott Hanrath, KU Libraries
- Patrice-Andre Prud'homme, OSU Library

---

Schedule:
- 9:10-10:00: Getting started with Git and Markdown
- 10:05-11:00: Collaborating using GitHub
- 11:05-12:00: Contributing to an open project using GitHub
- 12:05-12:30: Tour of the ArchivesSpace GitHub repository (with Scott Hanrath)

---

### Basics - navigating the command-line interface (also called the shell)

**`pwd`** print working directory

**`ls`** list directory

- `ls -l`: list a lot of file information
- `ls -lh`: list a lot of human-readable file information

**`cd`** change directory

---

### Basics - interacting with files on the command line

**`mkdir`** make directory

**`cat`** send file or files to output (in most cases, this shows the content of a file without having to open it)

**`head`** output first parts of a file or files (default is usually 10 lines)

**`tail`** output last parts of a file or files (default is usually 10 lines)

**`mv`** rename or move a file or files. Syntax for renaming a file: `mv FILENAME NEWFILENAME`  **USE WITH CAUTION!!!**

**`cp`** copy a file or files. Syntax: `cp FILENAME NEWFILENAME`

**`>`** redirect output. Syntax with `cat`: `cat FILENAME1 FILENAME2 > NEWFILENAME`

**`rm`** remove a file or files. **USE WITH CAUTION!!!**

---

### Basic Git commands 

**`git init`**: creates a git repository

**`git status`** : view the status of your files in the working directory and staging area

**`git add`**: tells git to start tracking a file, or a series of files. 

**`git commit`**: commits (saves) the staged snapshot to the project history. 

**`git log`**: shows all the commits in the project history

**`git diff`**: shows changes made to files

**`git remote add origin`**: add a remote repository where changes will be stored, usually for collaboration

**`git push`**: sends local changes to a remote repository

**`git pull`**: brings changes made in a remote repository to the local repository 

---

### Exercises

#### Exercise 1: Add to your Markdown cheat sheet

Edit your `index.md` file using a plain text editor. If you don't like working with nano on the command line you can open the file with Notepad (Windows) or TextEdit (Mac). If you use TextEdit you may need to change the document to plain text (Format > Make Plain Text).

Add the lines below to the file, leaving an empty line between the existing content and the new stuff. Try to type as much of this as you can, but if time is short you can copy/paste from the shared notes. Once you have added content to your file, save and close it, then add and commit it to your git repository.

`## Level 2 Heading`

`### Level 3 Heading`

`A paragraph is denoted by white space before and after.`

	A bulleted list:
	- level 1
	- level 1
			- level 2
			- level 2

	A numbered list:
	1. One
	2. Two
	3. Three

`*italic text*`

`**bold text**`

`~~strikethrough text~~`
  
	---
	Make a horizontal rule
	---

`Embed a link with [square brackets](https://daringfireball.net/projects/markdown/syntax)`

---

#### Exercise 2: Collaborate via GitHub
1. Complete this exercise with one partner:
   - Pair up
   - Share GitHub names
   - Decide which role you will play first, Owner or Collaborator
   - When you finish (after step 6), switch roles and complete the exercise again
2. Owner, invite the collaborator to contribute to your hello-world repository:
   - Click  Settings on the far right tab in your repository.
   - Click Collaborators, the second choice on the left menu.
   - Search for your collaborator using their GitHub name.
   - When you've found them, click Add Collaborator next to the search box.
3. Collaborator, accept the invitation:
   - Go to GitHub Notifications at [https://github.com/notifications](https://github.com/notifications) and accept the invitation.
   - Or open the email from GitHub in the address you used to create your account.
   - You should now have access to edit the repository.
4. Collaborator, find the Owner's `README.md` file. Edit the file and commit the changes.
5. Owner, refresh your browser and see the changes made by the Collaborator.
6. Both partners, click on the Commits link below the repository description. Explore the repository's commit history now that two people have made changes.
   
#### Exercise 2a: Optional steps

*The Collaborator has the option to create a local copy of the Owner's repository and edit the files there, then push changes to GitHub. This isn't necessary for today's exercise but it's handy to know how to do. Follow the instructions below or save them for your next Git/GitHub collaboration.*

1. Collaborator, go to the Owner's repository in GitHub and click the green Clone or download button on the far right.
2. Collaborator, copy the URL you find there.
3. Collaborator, switch to your command line interface and go to your Desktop:
   - **`cd ~/Desktop`**
4. Collaborator, download a copy of the Owner's repository to a folder on the Desktop of your computer:
   - **`git clone https://Owners-GitHub-Repo ~/Desktop/owner-hello-world`** 
   - Substitute the URL that you copied in step 2 for the placeholder text in the command
   - Substitute the Owner's name for "owner" in the folder name, e.g.: **`~/Desktop/jill-hello-world`**
5. Collaborator, you can change things in your clone of the Owner's repository:
   - **`cd ~/Desktop/owner-hello-world`**
   - **`nano README.md`** (or use your favorite text editor)
   - Make some changes to the file
   - Save and exit
   - **`git add README.md`**
   - **`git commit -m "Write a good commit message"`**
6. Collaborator, push your changes to the Owner's repository on GitHub:
   - **`git push origin master`**
   - We don't need to create a remote because Git does this automatically when we clone a repository
7. Both partners can look at the Owner's hello-world repository (maybe refresh your browser) and see the Collaborator's changes.
8. Owner, you need to get your local hello-world repository in sync with the remote now that your collaborator has made and pushed some changes.
   - Switch to your command line interface
   - Make sure that you are in your hello-world directory. Use **`pwd`** to see where you are and **`cd`** to move, if necessary.
   - **`git pull origin master`**
   - **`cat README.md`** (if you want to see that the changes are present)
9. All three repositories should be in sync. Switch roles and repeat.


*For another exercise using this collaboration model of two local repositories and one shared remote repository, check out Software Carpentry's "Version Control with Git: Conflicts" lesson at [http://swcarpentry.github.io/git-novice/09-conflict/](http://swcarpentry.github.io/git-novice/09-conflict/). The directory and file names are different but the concepts are the same.*

---

#### Exercise 3: Contributing to an open project using GitHub

1. Navigate to the repository: [https://github.com/kulibraries/20181130-gh-contribute](https://github.com/kulibraries/20181130-gh-contribute)
2. Claim an Issue by replying to it (this is optional when working on open projects outside of the workshop)
3. Click on the Fork button at the top right of the screen to make your own copy. You may be asked to choose where to fork (copy) the repository. Fork it into your own GitHub account. 
4. In your fork of the project, create a new branch. Pull down the Branch indicator and start typing to create a new branch. Name the branch for the change you intend to make, e.g.: `revise-cocktail-recipes` (avoid spaces in your branch names!).
5. In your fork, on your new branch, make your intended edit(s). This is a good chance to practice Markdown. Before you commit, you can preview how the file will look by clicking the Preview tab over the file. Note that you are learning GitHub-flavored Markdown; the syntax of other flavors of Markdown will be slightly different.
6. When you have finished your edits, commit (save) your changes. Be sure to write a good commit message.
7. Ask for the owner of the project to incorporate your changes into the project files by creating a pull request. This slightly confusing terminology basically means you REQUEST that the owner of the original source PULL your changes into their version. Follow these steps:
   - Go back to the Code tab of your forked repository
   - Confirm that you are using the branch that contains your edits. If the Branch indicator says `master` pull it down and change it.
   - Click New Pull Request right beside the branch indicator.
   - Compare the two repositories:
     - Base fork: the original project you forked (in this exercise, `kulibraries/20181130-gh-contribute`)
     - Base: the branch of the base fork (in this exercise,  `master`)
     - Head fork: YOUR fork (copy) of the project
     - Compare: name of branch (in this exercise, should be the name of your new branch, e.g.: `revise-cocktail-recipes`)
   - GitHub will indicate whether there are conflicts (there shouldn't be for this exercise). If there are no conflicts, you will see the green Create Pull Request button.
   - Click Create Pull Request
   - By default, your summary is the same as your commit message. Use the box below to explain the changes you made in more detail. This message should give the project owner a good idea of what changes you made and why.
     - Cite the Issue you addressed by typing `Issue #`
     - GitHub will give you a set of issues to pick from. Choose the issue you worked on.
   - Click the green Create Pull Request button at the bottom
8. GitHub will notify you if your pull request is accepted into the project.   

---

### Resources

**Library Carpentry Intro to Git lesson:** [https://librarycarpentry.org/lc-git/](https://librarycarpentry.org/lc-git/)

**GitHub Guides Hello World exercise:** [https://guides.github.com/activities/hello-world/](https://guides.github.com/activities/hello-world/)

**Mozilla Science Lab GitHub for Collaboration on Open Projects lesson:** [http://mozillascience.github.io/working-open-workshop/github_for_collaboration/](http://mozillascience.github.io/working-open-workshop/github_for_collaboration/)

**Software Carpentry Version Control with Git lesson** (offers more focus on command-line Git): [http://swcarpentry.github.io/git-novice/](http://swcarpentry.github.io/git-novice/)

**Step-by-step description of GitHub Flow for open projects** (specifically for Software Carpentry): [https://github.com/dmgt/swc_github_flow/blob/master/for_novice_contributors.md](https://github.com/dmgt/swc_github_flow/blob/master/for_novice_contributors.md)

---

### Source 
Author: Jamene Brooks-Kieffer

Affiliation: University of Kansas Libraries

Link: [https://github.com/kulibraries/20181130-gh-contribute/blob/master/git-handout.md](https://github.com/kulibraries/20181130-gh-contribute/blob/master/git-handout.md)

License: CC-BY [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)

Modified from James Baker's original Library Carpentry Git handout:
[https://github.com/LibraryCarpentry/week-three-library-carpentry-DEPRECATED/blob/master/handout.docx](https://github.com/LibraryCarpentry/week-three-library-carpentry-DEPRECATED/blob/master/handout.docx)

