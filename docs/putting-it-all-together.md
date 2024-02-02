---
marp: true
theme: uncover
_class: invert
---

# Git, GitHub, and Jupyter

Ty Janoski
City College of New York, CUNY 

---

## Let's set up a workflow for your in-class project.

---

### Creating a GitHub repository

Have *one* member of your group create a repository. This person will be the owner.<sup> * </sup>
<br></br>
<sup> * The owner doesn't have any special responsibilities, so don't worry. </sup>

---

![width:800px](nav-to-repos.png)

---

![width:800px](new-repos.png)


---

- Pick a name for your repository, like `SUSC`.
- Give it a short description.
- Leave it public.
- You can skip the `README`, `.gitignore`, and license for now.

--- 

![width:800px](create-repos.png)

---

### Invite your group members as collaborators

![width:700px](invite-collabs.png)

---

Create a new folder on your computer where your Jupyter Notebook for this class will live.

<br></br>

Make sure you can navigate to it using JupyterLab!

---

### Initialize a new repository

![width:700px](init-repos.png)

---

### Create a new notebook

- When selecting the kernel, make sure it is `susc`
- In your first cell, run this code:
`!git branch -m main`
- This just renames the branch from `master` to `main`

---

### Add your notebook

Hit the plus sign.

![width:700px](add-to-repo.png)

---

### Commit the changes
An example summary is "`added my first file`"

![height:400px](commit.png)

---

### Connect to remote repository

In the top menu bar, git -> manage remote

![width:500px](manage-remote.png)

---

### Push to GitHub

![width:600px](git-push.png)

---

### If it worked, refresh your GitHub repository page and see your file there now!

---

### Now it's time for branches.

Create a new branch for each group member.

---

### Click on branches.

![](branch-link.png)

---

### Make a new branch.

![width:800px](new-branch.png)

---

### Create branches for each group member including the owner!

![width:900px](branch-list.png)

---

### Now, the other members can clone the repository.

![width:700px](git-link.png)

---

### Paste the git link into the `git clone` dialog box

![width:700px](git-clone.png)

---

### When you work on this group project, make sure you are in *your* branch!

---

When you are ready to merge your changes into the `main` branch, make a pull request.

![width:700px](start-pull-request.png)

---

### Open a pull request

![width:800px](open-pull-request.png)

---

### Merge pull request

![width:700px](merge-pull-request.png)

