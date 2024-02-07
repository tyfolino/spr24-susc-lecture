---
marp: true
theme: uncover
_class: invert
---

# Git, GitHub, and Jupyter
## Lecture Notes

Ty Janoski
City College of New York, CUNY 

---

## Learning objectives:

- Understand **version control** and its role in collaborative software development.

- Learn to effectively use **Jupyter notebooks** for data analysis and collaborative documentation.

- Develop skills to set up and manage **collaborative workflows** with Git/GitHub and Jupyter for group projects.

---

## An introduction to version control

---

![height:600px](http://www.phdcomics.com/comics/archive/phd101212s.gif)

---

> Version control is the practice of tracking and managing changes to software code.

---

## Git
- Git: version control system
    - tracks changes to code over time
    - enables recall of specific versions
- Makes it easier for developers to work together
    - Lets users create *branches* to work independently and then *merge* the changes back into the main code
    - Each developer has a local copy of the code

---

### Git basics

1) Add file(s) to a staging area.
`git add somefile.py`
2) Save changes to a *local* repository.
`git commit -m "Made some awesome changes!"`
3) (Opt.) Upload changes to *remote* repository.
`git push`

---

![](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

---

# Git is helpful on its own

### But it really shines when used with GitHub!

---

# GitHub

![](https://play-lh.googleusercontent.com/PCpXdqvUWfCW1mXhH1Y_98yBpgsWxuTSTofy3NGMo9yBTATDyzVkqU580bfSln50bFU)

---

# GitHub

GitHub is a website where you can host your code & files in databases called "repositories."
<br></br>
<sup>I don't fully understand how GitHub gets money but they offer tons of services for free.</sup>

---
## Typical GitHub workflow
![](Distributed-Version-Control-System-edited.jpg)

---

### We can go the other way, too.

- `git clone github.com/somerepository.git`
    - Creates a copy of an entire remote repository
- `git pull`
    - "Pulls" the latest changes and commits from the remote repository to your local working copy

Typically, you only `clone` once but `pull` many times.

---

### So far, the workflows we've described are good for people working by themselves, but in this class and in the future, you will be working on a team.

---

## Branching

In Git/GitHub, branching creates **a parallel version of the code** to work on new features or fixes *without affecting the main codebase*. It allows developers to isolate their work, make changes, and then merge those changes back into the main code when they are ready.

---



## Branching
![](Distributed-Version-Control-System.jpg)

---

### Branching workflow

- Create and switch to branch
`git checkout -b new-branch`
- Add changes and commit
`git add ...`
`git commit -m "..."`
- Push branch to GitHub
`git push -u origin new-branch`<sup>*</sup>

<sup>* after the first push, you can just use `git push`</sup>

---

### If you want to merge changes from a branch to the main code...
- Start a **pull request**
- Review & merge

---

## Pull requests

A pull request is a way to propose changes from a branch in a repository to the main code. It allows developers to notify others about the changes they've made, discuss modifications, and eventually merge the changes into the main code.

---

### Pull requests

![width:900px](https://www.atlassian.com/blog/wp-content/uploads/bitbucket411-blog-1200x-branches2.png)

---

## Other helpful git tools
- `git status` = check status of your files
- `git branch` = list branches
- `git rm` = delete a file
- `git stash` = temporarily store your changes
- `git checkout <branchname>` = switch branches
- `git stash pop` = apply changes to current branch

---

Version control with Git and GitHub can be confusing. You don't need to understand everything right now to develop a collaborative workflow for this class 😁.

---

## Resources/References

- [Learn git branching](https://learngitbranching.js.org/?locale=en_US)
- [Git/GitHub Lecture by Madicken Munk](https://munkm.github.io/2024-winterschool/git-collaboration.slides.html#/)
- [GitHub Docs](https://docs.github.com/en)
- [The Git book](https://git-scm.com/book/en/v2)