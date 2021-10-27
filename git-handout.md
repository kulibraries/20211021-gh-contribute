# Introduction to GitHub

## Topics in Environmental Studies: Team Science
### University of Kansas
### October 28, 2021

---

Personnel:
- Jamene Brooks-Kieffer, KU Libraries
- Samantha Thomas, Kansas Biological Survey

---

### Exercise: Contributing to an open project using GitHub

1. Navigate to the repository: [https://github.com/kulibraries/20211021-gh-contribute](https://github.com/kulibraries/20211021-gh-contribute)
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
     - Base fork: the original project you forked (in this exercise, `kulibraries/20211021-gh-contribute`)
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

### A Markdown cheat sheet

Use the code below to add Markdown-formatted content to any file with a \*.md file extension, or create a new Markdown-formatted file. Use a plain text editor any time you work in Markdown; a word processor like MS Word will try to interpret your code for you. Useful and extensible text editors include:

- [Notepad++](http://notepad-plus-plus.org/) (Windows only)
- [Atom](https://atom.io/) (all OS)
- [Sublime Text](https://www.sublimetext.com/) (all OS)

Markdown can be incorporated into R using the [`rmarkdown`](https://rmarkdown.rstudio.com/index.html) package. Markdown can also be written into a [Jupyter Notebook or JupyterLab](https://jupyter.org/index.html) cell. All of these options are great for documenting your code.

Note that Markdown is sensitive to space characters and line breaks. If your Markdown isn't formatting as you expect, check your white space.

`# Level 1 Heading`

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

	`code text`

`~~strikethrough text~~`
  
	---
	Make a horizontal rule
	---

`Embed a link with [square brackets](https://daringfireball.net/projects/markdown/syntax)`

---

### Glossary of GitHub Jargon

**Branch**: A sandbox area for experimenting in the project without affecting the main production files.

**Commit**: Save your work

**Commit message**: A note you write to yourself/collaborators when you save

**Fork**: Make a copy of the repository; the new copy is still linked to the original

**History**: What happened to the project in the past - preserved in the repository and Commit messages

**Issue**: A task that needs doing in the GitHub repository, or a note left to the project owner

**Pull request**: A way to ask the project owner to incorporate your change into the original repository

**Repository** or **Repo**: The set of files that make up the project

---

### Resources

**GitHub Guides Hello World exercise:** [https://guides.github.com/activities/hello-world/](https://guides.github.com/activities/hello-world/)

**Mozilla Science Lab GitHub for Collaboration on Open Projects lesson:** [http://mozillascience.github.io/working-open-workshop/github_for_collaboration/](http://mozillascience.github.io/working-open-workshop/github_for_collaboration/)

**Step-by-step description of GitHub Flow for open projects** (specifically for Software Carpentry): [https://github.com/dmgt/swc_github_flow/blob/master/for_novice_contributors.md](https://github.com/dmgt/swc_github_flow/blob/master/for_novice_contributors.md)

**Software Carpentry Version Control with Git lesson** (offers more focus on command-line Git): [http://swcarpentry.github.io/git-novice/](http://swcarpentry.github.io/git-novice/)

**Library Carpentry Intro to Git lesson:** [https://librarycarpentry.org/lc-git/](https://librarycarpentry.org/lc-git/)

---

### Source 
Author: Jamene Brooks-Kieffer

Affiliation: University of Kansas Libraries

Link: [https://github.com/kulibraries/20211021-gh-contribute/blob/master/git-handout.md](https://github.com/kulibraries/20211021-gh-contribute/blob/master/git-handout.md)

License: CC-BY [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)

Modified from James Baker's original Library Carpentry Git handout:
[https://github.com/LibraryCarpentry/week-three-library-carpentry-DEPRECATED/blob/master/handout.docx](https://github.com/LibraryCarpentry/week-three-library-carpentry-DEPRECATED/blob/master/handout.docx)

Also adapted from the Mozilla Science Lab GitHub for Collaboration on Open Projects lesson: [http://mozillascience.github.io/working-open-workshop/github_for_collaboration/](http://mozillascience.github.io/working-open-workshop/github_for_collaboration/)
