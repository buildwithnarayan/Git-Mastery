# Why Git?

**Estimated Reading Time:** 10–15 minutes

---

# 💡 Did You Know?

Git was created by **Linus Torvalds**, the creator of the Linux kernel, in **2005**.

He designed Git in just a few weeks after the Linux community lost access to the proprietary version control system they were using.

Today, Git is the world's most widely used Version Control System.

---

# Learning Objectives

By the end of this chapter, you will:

* Understand why Git was created.
* Learn the limitations of older Version Control Systems.
* Understand why Git became the industry standard.
* Learn the design goals behind Git.

---

# Imagine This...

It's 2005.

You are one of hundreds of developers contributing to the Linux kernel.

Thousands of files change every day.

Developers work from different countries and time zones.

Creating a branch takes several minutes.

Merging code is slow.

If the central server becomes unavailable, nobody can commit changes.

The development process is becoming increasingly difficult.

A better solution is needed.

---

# The Problem Before Git

Before Git, many teams used Centralized Version Control Systems such as **CVS** and **Subversion (SVN)**.

Although they solved many problems compared to manually copying files, they introduced new challenges:

* Every operation depended on a central server.
* Branching was relatively slow.
* Merging large projects was difficult.
* Working offline was limited.
* A central server outage affected the entire team.

As software projects became larger, these limitations became more noticeable.

---

# Why Did Linus Torvalds Create Git?

The Linux kernel is one of the largest open-source software projects in the world.

Linus Torvalds needed a system that was:

* Extremely fast
* Reliable
* Distributed
* Easy to branch
* Easy to merge
* Able to handle thousands of contributors

Existing tools did not meet all these requirements.

So he created Git.

---

# Git's Design Goals

Git was designed with a few clear principles:

## Speed

Most Git operations happen locally, making commands like `status`, `log`, and `branch` extremely fast.

---

## Distributed Development

Every developer has a complete copy of the repository.

This means you can:

* Work offline
* View history locally
* Create commits without an internet connection

---

## Reliable History

Every commit is identified by a unique cryptographic hash.

If the content changes, the hash changes.

This helps protect the integrity of the project's history.

---

## Powerful Branching

Creating a branch in Git is extremely lightweight.

Branches allow developers to experiment safely without affecting the main codebase.

---

# Industry Insight

Today, Git powers some of the world's largest software projects, including:

* Linux Kernel
* Kubernetes
* Docker
* VS Code
* React
* TensorFlow

Millions of developers rely on Git every day.

---

# Real-World Example

Imagine a company with 500 developers.

Each developer works on a separate feature.

Using Git:

* Every feature is developed in its own branch.
* Code is reviewed using Pull Requests.
* Changes are merged only after approval.
* Production remains stable while new features are developed.

This workflow would be difficult to manage efficiently without Git.

---

# Hands-on Exercise

Answer these questions:

1. Why was Git created?
2. What problems did older Version Control Systems have?
3. Which Git design goal do you think is most important, and why?

---

# Common Misconceptions

❌ Git was created only for Linux.

❌ Git requires an internet connection to work.

❌ GitHub created Git.

---

# Interview Questions

### Beginner

* Who created Git?
* When was Git created?

### Intermediate

* Why was Git developed?
* What problems did Git solve?

### Advanced

* Why is Git considered a Distributed Version Control System?
* Explain the design principles behind Git.

---

# Key Takeaways

* Git was created by Linus Torvalds in 2005.
* Git was designed to be fast, distributed, and reliable.
* Git solved many limitations of older Version Control Systems.
* Today, Git is the industry standard for software development.

---

# What's Next?

In the next chapter, we'll answer one of the most common interview questions:

**What is the difference between Git and GitHub?**

Although many people use the terms interchangeably, they are very different technologies with different purposes.

---

⬅️ Previous: [Version Control](02-Version-Control.md)

➡️ Next: [Git vs GitHub](04-Git-vs-GitHub.md)

