---
marp: true
theme: uncover
class: invert
---

# Git, GitHub, and Jupyter

Ty Janoski
City College of New York, CUNY 

---

# Before we talk about Git...

## We have to talk about version control.

---

![height:600px](http://www.phdcomics.com/comics/archive/phd101212s.gif)

---

# Basics of version control

1) Add file(s) to a staging area.
`git add myfile.py`
2) Write changes to a local repository.
`git commit -m "made some changes"`
3) (Opt.) Push changes to *remote* repository.
`git push -u origin main`

Note: while it's good to know these commands, we will use a GUI to make it easier.

---

![](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

---

# Git is helpful on its own:

- It lets you easily track changes to your code
- If something goes wrong, you can rollback to an earlier, working version
- You can organize your tasks and workflow ("branching")

### But it really shines when used with GitHub!

---

# GitHub

![](https://play-lh.googleusercontent.com/PCpXdqvUWfCW1mXhH1Y_98yBpgsWxuTSTofy3NGMo9yBTATDyzVkqU580bfSln50bFU)

---

# GitHub

GitHub is a website where you can host your code & files in databases called "repositories."
<br></br>
<sup>I don't fully understand how GitHub gets money but they offer tons of services for free. No need to question it!</sup>

---

![](https://media.geeksforgeeks.org/wp-content/uploads/20191203164948/Distributed-Version-Control-System.jpg)

---

## Here's a typical workflow.
1) `git add your-files-here.txt` to add your files and edits to the staging area
2) `git commit -m "your message here"` to put these updated files to your *local* repository
3) `git push` your changes to GitHub repository

Note: Before pushing the first time, we will have to connect our Git and GitHub repositories.

---

# A small task before our hands-on exercises

---

On whatever terminal you've been using (Windows Powershell, MacOS terminal, Windows terminal, Anaconda prompt, Spyder console, etc...), enter the following:
`git config --global user.name "First Last"`
and
`git config --global user.email "your-github-email@example.com"`

Make sure you use the same email on your GitHub account!

---

# In case people are having authentication issues...

----

### Authentication to remote repository hosts

If you are seeing errors similar to `[E yyyy-mm-dd hh:mm:ss ServerApp] 500 POST /git/<clone|push|pull|status>` on the console which is running the JupyterLab server, you probably need to set up a credentials store for your local Git repository.

This extension tries to handle credentials for HTTP(S) connections (if you don't have set up a credential manager). But not for other SSH connections.

---

### A note for windows users. 

> For Windows users, it is recommended to install [git for windows](https://gitforwindows.org/). It will automatically set up a credential manager.
> In order to connect to a remote host, it is recommended to use SSH.

---


#### SSH protocol

Here are the steps to follow to set up SSH authentication (skip any that is already accomplished for your project):

1. [Create a SSH key](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Register the public part of it to your Git server:
   - [GitHub](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)


---

3. Tell your local Git repository to [connect to remote via ssh](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories#switching-remote-urls-from-https-to-ssh)
<br></br>

You should now be able to pull and push committed changes to and from your remote repository using the respective buttons on the top of the extension's panel.