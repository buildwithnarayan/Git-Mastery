# Version Control

**Estimated Reading Time:** 10–15 minutes

---

# Learning Objectives

By the end of this chapter, you will:

- Understand what Version Control is.
- Learn why Version Control is important.
- Understand the problems it solves.
- Learn the different types of Version Control Systems.
- Understand why modern software teams rely on Version Control.

---

# Imagine This...

You are working on your college final-year project.

On Day 1, your project folder looks like this:

```text
EmployeeManagementSystem
```

After making a few changes, you create another copy:

```text
EmployeeManagementSystem_Final
```

A week later:

```text
EmployeeManagementSystem_Final_v2
```

The night before submission:

```text
EmployeeManagementSystem_Final_v2_Latest
EmployeeManagementSystem_Final_v2_UseThisOne
EmployeeManagementSystem_Final_v2_Final_Final
```

Now imagine asking yourself:

- Which version is the latest?
- Which version contains the bug fix?
- Which version should I submit?

This is exactly the problem Version Control solves.

---

# What is Version Control?

Version Control is a system that records changes to files over time, allowing you to:

- Track every modification.
- Restore previous versions.
- Compare changes.
- Collaborate with other developers.
- Understand who changed what and when.

Instead of creating multiple copies of files, Version Control keeps a structured history of your project.

---

# Why Do We Need Version Control?

Without Version Control:

- Files get overwritten.
- Multiple copies of the same project are created.
- Collaboration becomes difficult.
- Recovering previous versions is almost impossible.
- Finding the source of a bug takes longer.

With Version Control:

- Every change is recorded.
- Previous versions are always available.
- Team collaboration becomes much easier.
- Mistakes can often be reversed safely.
- Development becomes organized and predictable.

---

# Types of Version Control Systems

## 1. Local Version Control

Everything is stored on your own computer.

Advantages:

- Simple
- Fast

Disadvantages:

- No collaboration
- Easy to lose data if your computer fails

---

## 2. Centralized Version Control (CVCS)

Examples:

- SVN
- CVS

All developers connect to one central server.

Advantages:

- Easy to manage
- Everyone works from one central repository

Disadvantages:

- If the server goes down, work stops.
- Internet access is usually required.

---

## 3. Distributed Version Control (DVCS)

Examples:

- Git
- Mercurial

Every developer has a complete copy of the repository.

Advantages:

- Work offline
- Faster operations
- Better collaboration
- Full project history on every machine

Git belongs to this category.

---

# Real-World Example

Imagine a company with 50 developers.

Without Version Control:

- Developers overwrite each other's work.
- Bugs are difficult to trace.
- Releases become risky.

With Git:

- Every developer works on their own branch.
- Code is reviewed before merging.
- Every change has a history.
- Production releases are easier to manage.

---

# Industry Insight

Today, Version Control is not only used for application source code.

Modern teams also version control:

- Infrastructure as Code
- Kubernetes manifests
- Terraform configurations
- Documentation
- CI/CD pipelines
- Database scripts

If it is important, it should be version controlled.

---

# Hands-on Exercise

Think about a project you have worked on.

Answer these questions:

1. How did you manage different versions?
2. Did you create multiple copies?
3. Could you easily restore yesterday's version?
4. How would Git have improved your workflow?

---

# Common Mistakes

❌ Using filenames to manage versions.

❌ Sharing projects over email.

❌ Editing the same file simultaneously without Version Control.

---

# Interview Questions

### Beginner

- What is Version Control?
- Why do we need Version Control?

### Intermediate

- What are the different types of Version Control Systems?
- Why is Git called a Distributed Version Control System?

### Advanced

- Explain the advantages of Distributed Version Control over Centralized Version Control.

---

# Key Takeaways

- Version Control records every change made to a project.
- It simplifies collaboration.
- It helps recover previous versions.
- Git is a Distributed Version Control System.
- Version Control is a fundamental skill for every software professional.

---

# What's Next?

In the next chapter, we'll answer an important question:

**Why was Git created when other Version Control Systems already existed?**

---

⬅️ Previous: [Git Introduction](01-Introduction-to-Git.md)

➡️ Next: [Why Git?](03-Why-Git.md)
