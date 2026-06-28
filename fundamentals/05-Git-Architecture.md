# Git Architecture

**Estimated Reading Time:** 15–20 minutes

---

# 💡 Did You Know?

Many developers use Git for years without knowing where commits are actually stored.

One of Git's biggest strengths is that it stores everything inside a hidden directory called `.git`.

Understanding this directory will help you become confident with advanced Git concepts like branching, merging, rebasing, and recovering lost work.

---

# Learning Objectives

By the end of this chapter, you will:

* Understand the architecture of a Git repository.
* Learn the purpose of the `.git` directory.
* Understand the Git workflow.
* Learn how Git stores project history.
* Understand the relationship between the Working Directory, Staging Area, and Local Repository.

---

# Imagine This...

You create a new project:

```bash
mkdir MyProject
cd MyProject
git init
```

After running `git init`, a hidden folder appears:

```text
.git/
```

This small folder is the heart of Git.

It contains everything Git needs to manage your project.

Without it, your project is just a normal folder.

---

# The Three Areas of Git

Every change you make moves through three stages.

```text
                Working Directory
                        │
                 git add
                        │
                        ▼
                Staging Area
                        │
               git commit
                        │
                        ▼
              Local Git Repository
                        │
                 git push
                        │
                        ▼
             Remote Repository (GitHub)
```

Understanding this flow is one of the most important concepts in Git.

---

# Working Directory

The Working Directory is where you create and edit files.

Example:

```text
EmployeeService.java
README.md
Dockerfile
```

Changes made here are not yet tracked by Git.

---

# Staging Area

The Staging Area acts as a preparation area.

When you run:

```bash
git add EmployeeService.java
```

Git prepares that file to be included in the next commit.

This gives you control over what is included in each commit.

---

# Local Repository

When you run:

```bash
git commit -m "Add employee service"
```

Git stores a snapshot of the staged changes in the local repository.

This history is stored inside the `.git` directory.

At this point, the commit exists only on your computer.

---

# Remote Repository

When you run:

```bash
git push
```

Your local commits are uploaded to a remote repository, such as GitHub.

This makes them available to other developers.

---

# What's Inside the .git Directory?

Run:

```bash
ls -la .git
```

You'll see files and folders similar to:

```text
HEAD
config
objects/
refs/
hooks/
logs/
index
```

Some important components are:

* **HEAD** – Points to your current branch.
* **objects/** – Stores commits, files, and trees.
* **refs/** – Stores branch references.
* **config** – Repository-specific configuration.
* **index** – Represents the Staging Area.

Don't worry if these names are unfamiliar. We'll explore them in later chapters.

---

# Real-World Example

Imagine you're developing a new login feature.

You edit several files.

Those changes exist only in your Working Directory.

You stage selected files:

```bash
git add .
```

Now Git knows which changes should become part of the next commit.

After reviewing your work, you commit:

```bash
git commit -m "Implement login feature"
```

The commit is safely stored in your local repository.

Finally:

```bash
git push
```

shares your work with the team.

---

# Industry Insight

Every modern CI/CD pipeline begins with Git.

A push to GitHub can automatically trigger:

* Jenkins pipelines
* GitHub Actions
* GitLab CI
* Docker image builds
* Kubernetes deployments

Git is often the starting point of an automated software delivery pipeline.

---

# Hands-on Exercise

Create a new repository and observe Git's architecture.

```bash
mkdir git-architecture-demo
cd git-architecture-demo
git init
ls -la
ls -la .git
```

Identify:

* The hidden `.git` directory
* The `HEAD` file
* The `objects` directory

---

# Common Mistakes

❌ Thinking commits are stored on GitHub.

❌ Forgetting the Staging Area exists.

❌ Assuming `git add` creates a commit.

❌ Believing Git automatically uploads commits.

---

# Interview Questions

### Beginner

* What is the `.git` directory?
* What are the three areas of Git?

### Intermediate

* What happens after running `git add`?
* What happens after `git commit`?

### Advanced

* What information is stored inside `.git/objects`?
* Why is the Staging Area useful?

---

# Key Takeaways

* Git stores repository data inside the hidden `.git` directory.
* Every change flows through the Working Directory, Staging Area, and Local Repository.
* `git push` sends local commits to a remote repository.
* Understanding Git's architecture makes advanced Git much easier to learn.

---

# What's Next?

In the next chapter, we'll install Git, configure it properly, and create our first repository from scratch using best practices.

---

⬅️ Previous: [Git vs GitHub](04-Git-vs-GitHub.md)

➡️ Next: [Git Installation](06-Installing-Git.md)
