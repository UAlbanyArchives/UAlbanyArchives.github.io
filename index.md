<style>
#cli-path {color:red}
#gui-path {color:yellow}
</style>

## Git and GitHub for Libraries

Greg Wiedeman and Mark Wolfe

M.E. Grenander Department of Special Collections & Archives

University at Albany, SUNY

---

## Stuff to Do

* Make a [Github Account](https://github.com/login)
* Download and install [Git](https://git-scm.com/) or [Github Desktop](https://desktop.github.com//)
* Download and install markdown editor (optional)
	* [Typora](https://typora.io/)
	* [Atom](https://atom.io/)
	* [Markdown Pad](http://markdownpad.com/) (Windows)
	* [Mou](http://25.io/mou/) (Mac/Linux)
	* [MacDown](https://macdown.uranusjr.com/) (Mac/Linux)

---

<p>1. [Create a Github Account](https://github.com/join?source=login) or [Login](https://github.com/login) to your existing account.</p>

![Join Github](img/join.png)

---

<p>2. [Create a new git repository](https://github.com/new)</p>


![new git repository](img/newrepo.png)

---

<p>3. Enter USERNAME.github.io</p>


![new git repository](img/newrepo2.png)

---

<p>4. This is your Github Repository</p>


![new git repository](img/newrepo3.png)

---

### CLI Path
<p>5. [Download and Install Git](https://git-scm.com/)</p>


![new git repository](img/downloadgit.png)

---

### GUI Path
<p>5. [Download and Install Github Desktop](https://desktop.github.com//)</p>


![new git repository](img/githubdesktop.png)

---

### GUI Path
<p>5. Tell Git who you are</p>

		git config --global user.email "you@example.com"
		git config --global user.name "Your Name"

---

### CLI Path
<p>6. Clone your repo</p>
* Open Terminal, Powershell or cmd.exe


		git clone http://github.com/USERNAME.github.io

* Change directory into your repo


		cd USERNAME.github.io

![Clone repo](img/clone.png)

---

### GUI Path
<p>6. Clone your repo</p>

![Clone repo in Github Desktop](img/clonedesktop.png)

---

### CLI Path
<p>7. Open your repo</p>
* Windows:

		start .

* Mac OSX/Linux:

		open .


---

### GUI Path
<p>7. Open your repo</p>

![open repo](img/openrepo.png)


---

<p>8. Look at your repo</p>

![open repo](img/repo.png)

---

<p>9. (Optional) Install a Markdown Editor</p>

* Cross Platform:
	* [Atom](https://atom.io/)
	* [Typora](https://typora.io/)

* Windows:
	* [MarkdownPad 2](http://markdownpad.com/)

* Mac OSX/Linux
	* [Mou](http://25.io/mou/)
	* [MacDown](https://macdown.uranusjr.com/)

---

<p>10. Edit README.md ([Markdown CheatSheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet))</p>

![open repo](img/readme.png)

---

### CLI Path

<p>11. See the Changes</p>

		git status

---

### CLI Path

<p>11. Add, Commit, Push</p>

		git add .
		git commit -m "Updated Readme!"
		git push origin master

---

### GUI Path

<p>11. Add, Commit, Push</p>

![open repo](img/addchanges.png)

---

<p>12. Take a look at your commit!<p>

![Look at your commit!](img/commit.png)

---

<p>13. Make a bad edit<p>

![This is a mistaken commit.](img/mistake1.png)

---

### CLI Path

<p>14. Commit your mistake<p>

		git add .
		git commit -m "this is a mistake"
		git push origin master

---

### GUI Path

<p>14. Commit your mistake<p>

![A mistake commit.](img/mistake.png)

---

### CLI Path

<p>14. Revert!<p>

		git revert commitID
		:quit
		git push origin master


---

### GUI Path

<p>14. Revert!<p>

![A mistake commit.](img/revert.png)

---

## Collaboration

![Github Model](http://3.bp.blogspot.com/-SnWr9oa-G30/UY6tZKwGZPI/AAAAAAAABLc/dyQGoX_i3E8/s800/Github.png)

---

## Collaboration Concepts

* Pull Request
	* A suggested change
* Branch
	* A separate version of a repo
* Merge
	* Combining a "branch" with the "master" 
* Fork
	* Your personal copy of a repo
	* For pull requests when you are not a collaborator

---

### CLI Path

<p>15. Checkout a Branch and make a Pull Request</p>

		git checkout -b myNewBranch
		git add .
		git commit -m "the changes to my branch"
		git push origin myNewBranch

---

### GUI Path

<p>15. Checkout a Branch and make a Pull Request</p>


---

## Use Case: Collecting Policy

* [UAlbany Archives Collection Development Policy](http://library.albany.edu/archive/policy)
* [Rockefeller Archive Center Digital Team Values](https://github.com/RockefellerArchiveCenter/dteamValues/blob/master/values.md)
* [DACS Content Standard](https://github.com/saa-ts-dacs/dacs)
![Collection Development Policy in Markdown](img/policy.png)

---

## Use Case: Collecting Policy

* Converting markdown with [pandoc](https://pandoc.org/)


		pandoc policy.md -s -o policy.html
		pandoc policy.md -s -o policy.docx
		pandoc policy.md -s -o policy.pdf



---

## Use Case: Metadata Versioning

* [UAlbany Archives EAD repo](http://github.com/ualbanyarchives/collections)
* [Example Commit](https://github.com/UAlbanyArchives/collections/commit/5504d25c5d5b7a6ca167fe01c2c8a4a4573adbc5)

---

## Use Case: Free Static Hosting

* [Collection Development Policy](http://ualbanyarchives.github.io/policy.html)
* Static Page Generation
	* [Jekyll](https://jekyllrb.com/)
	* [www.gregwiedeman.com](http://www.gregwiedeman.com/)
	* [gwiedeman.github.io](http://gwiedeman.github.io)
	* [https://github.com/gwiedeman/gwiedeman.github.io](https://github.com/gwiedeman/gwiedeman.github.io)
	* [StatidAid](http://hillelarnold.com/staticAid/)
	* [Boston College Libraries](https://github.com/BCLibraries/bc-libraries-site)

---

## Use Case: Slideshows!

* [Reveal.js](http://lab.hakim.se/reveal-js/#/)
* [Reveal-md](https://github.com/webpro/reveal-md)
* These slides were written in Markdown and are hosted by Github Pages!
	* [See the Markdown](https://ualbanyarchives.github.io/index.md/)