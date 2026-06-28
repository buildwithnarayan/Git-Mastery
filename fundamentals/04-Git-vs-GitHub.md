# Git vs GitHub

**Estimated Reading Time:** 10–15 minutes

---

# 💡 Did You Know?

One of the most common mistakes beginners make is thinking **Git** and **GitHub** are the same thing.

They are related, but they solve different problems.

Understanding the difference is essential before learning collaboration and remote repositories.

---

# Learning Objectives

By the end of this chapter, you will:

* Understand the difference between Git and GitHub.
* Learn when to use Git.
* Learn when to use GitHub.
* Understand how Git and GitHub work together.
* Recognize common misconceptions.

---

# Imagine This...

You're working on your laptop and writing a Java application.

You save your progress by creating commits.

Your friend asks:

> "Can you share your code with me?"

Your commits exist only on **your computer**.

How do you share them?

This is where GitHub comes in.

---

# What is Git?

Git is a **Distributed Version Control System (DVCS)**.

It runs **locally on your computer** and helps you:

* Track changes
* Create commits
* Create branches
* Merge changes
* View project history
* Restore previous versions

Git works perfectly even without an internet connection.

---

# What is GitHub?

GitHub is a **cloud-based platform** that hosts Git repositories.

It allows developers to:

* Store repositories online
* Collaborate with other developers
* Create Pull Requests
* Review code
* Track Issues
* Manage Projects
* Automate workflows using GitHub Actions

GitHub uses Git, but Git itself does not depend on GitHub.

---

# Git vs GitHub

| Git                    | GitHub                                       |
| ---------------------- | -------------------------------------------- |
| Version Control System | Git hosting platform                         |
| Installed locally      | Cloud platform                               |
| Works offline          | Used for collaboration                       |
| Creates commits        | Stores remote repositories                   |
| Creates branches       | Manages Pull Requests                        |
| Open source software   | Commercial platform with free and paid plans |

---

# How They Work Together

Think of Git and GitHub like writing a document.

* **Git** is like working on the document on your own computer.
* **GitHub** is like storing that document in a shared online workspace where your team can review and collaborate.

Typical workflow:

```text
Write Code
     │
     ▼
Git Commit (Local)
     │
     ▼
git push
     │
     ▼
GitHub Repository
     │
     ▼
Pull Request
     │
     ▼
Code Review
     │
     ▼
Merge
```

---

# Real-World Example

Imagine you're working as a DevOps Engineer.

You update a Jenkins pipeline.

First, you commit the change using Git:

```bash
git add .
git commit -m "Update Jenkins pipeline"
```

The commit exists only on your computer.

To share it with your team:

```bash
git push origin feature/jenkins-update
```

Now the branch is available on GitHub, where teammates can review your work and merge it.

---

# When Do You Use Git?

You use Git when you want to:

* Save your work
* Create commits
* Create branches
* Merge changes
* View history
* Recover previous versions

---

# When Do You Use GitHub?

You use GitHub when you want to:

* Share code
* Collaborate with teammates
* Open Pull Requests
* Review code
* Track Issues
* Manage releases
* Trigger CI/CD pipelines

---

# Industry Insight

Many companies use Git internally but do **not** use GitHub.

Other Git hosting platforms include:

* GitLab
* Bitbucket
* Azure DevOps

The Git concepts you learn remain the same regardless of the hosting platform.

---

# Common Misconceptions

❌ Git and GitHub are the same.

❌ Git requires GitHub.

❌ GitHub created Git.

❌ Git works only when connected to the internet.

---

# Hands-on Exercise

Answer the following:

1. Can you create commits without GitHub?
2. Can you use Git without an internet connection?
3. What happens when you run `git push`?
4. Why would a team use GitHub if Git already stores project history?

---

# Interview Questions

### Beginner

* What is Git?
* What is GitHub?
* What is the difference between Git and GitHub?

### Intermediate

* Can Git work without GitHub?
* What happens when you execute `git push`?

### Advanced

* Name three alternatives to GitHub.
* Explain how Git and GitHub complement each other in a software development workflow.

---

# Key Takeaways

* Git and GitHub are different technologies.
* Git manages version history locally.
* GitHub hosts Git repositories and enables collaboration.
* You can use Git without GitHub.
* GitHub builds on top of Git by providing collaboration features.

---

# What's Next?

In the next chapter, we'll look inside Git itself and answer an important question:

**How does Git store commits, branches, and project history internally?**

Understanding Git's architecture will make advanced topics like branching, merging, rebasing, and recovering lost commits much easier to understand.

---

⬅️ Previous: [Why Git?](03-Why-Git.md)

➡️ Next: [Git Architecture](05-Git-Architecture.md)
