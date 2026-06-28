# Your First Git Repository

**Estimated Reading Time:** 20–25 minutes

---

# 💡 Did You Know?

Every Git repository starts as a normal folder.

It only becomes a Git repository after you initialize it using:

```bash
git init
```

This command creates a hidden `.git` directory that stores all Git metadata.

---

# Learning Objectives

By the end of this lesson, you will:

- Create your first Git repository.
- Understand what `git init` does.
- Create and track files.
- Stage changes.
- Create your first commit.
- View commit history.
- Understand the role of the `.git` directory.

---

# Before We Begin

Imagine you're starting a brand-new project.

```
ExpenseTracker/
```

At this point, it's just a normal folder.

Git knows nothing about it.

---

# Step 1 – Create a Project

```bash
mkdir ExpenseTracker
cd ExpenseTracker
```

Verify your location:

```bash
pwd
```

---

# Step 2 – Initialize Git

```bash
git init
```

Example output:

```text
Initialized empty Git repository in .../ExpenseTracker/.git/
```

Congratulations!

Your project is now a Git repository.

---

# Step 3 – Inspect the Repository

List hidden files:

```bash
ls -la
```

You'll see:

```text
.git
```

This hidden directory stores:

- Commit history
- Branch information
- Repository configuration
- Object database

Without `.git`, your folder is just a normal directory.

---

# Step 4 – Create Your First File

```bash
touch README.md
```

Add some content:

```text
# Expense Tracker

Learning Git with BuildWithNarayan.
```

---

# Step 5 – Check Repository Status

```bash
git status
```

You'll see:

```text
Untracked files:

README.md
```

Git has noticed the file but is not tracking it yet.

---

# Step 6 – Stage the File

```bash
git add README.md
```

Check the status again:

```bash
git status
```

Now Git reports the file as ready to be committed.

---

# Step 7 – Create Your First Commit

```bash
git commit -m "docs: add initial README"
```

Congratulations!

You've created your first commit.

This snapshot is stored in your local Git repository.

---

# Step 8 – View Commit History

```bash
git log
```

Or the compact version:

```bash
git log --oneline
```

You'll see your first commit along with its unique commit ID.

---

# Understanding the Workflow

```
Create File
      │
      ▼
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
Local Repository
```

This workflow is the foundation of Git.

---

# 💼 Real DevOps Scenario

Imagine you're updating a Kubernetes deployment manifest.

You:

1. Edit the YAML file.
2. Check the changes with `git status`.
3. Stage only the relevant files.
4. Commit with a meaningful message.
5. Push the commit.
6. Open a Pull Request.

This exact workflow is followed every day in DevOps teams.

---

# Hands-on Lab

Complete these tasks:

1. Create a new repository.
2. Add a README.
3. Run `git status`.
4. Stage the README.
5. Commit it.
6. View the commit history.

---

# 🎯 Challenge Exercise

Create a repository named:

```
git-practice
```

Inside it:

- Create `README.md`
- Create `notes.txt`

Stage **only** `README.md`.

Run:

```bash
git status
```

Can you explain why `notes.txt` is still untracked?

---

# 🧠 Think Like Git

Question:

After running:

```bash
git add README.md
```

Has Git created a commit?

**Answer:** No.

The file has only moved to the **Staging Area**.

---

# Common Mistakes

❌ Forgetting to initialize the repository.

❌ Forgetting to stage files before committing.

❌ Creating commits with messages like:

```
changes
```

Instead, write meaningful commit messages such as:

```
docs: add project README
```

---

# Interview Questions

### Beginner

- What does `git init` do?
- What is the purpose of the `.git` directory?
- What does `git status` show?

### Intermediate

- What happens when you run `git add`?
- What is the difference between an untracked and a staged file?

### Advanced

- Why is the Staging Area useful?
- Explain the complete Git workflow from creating a file to creating a commit.

---

# Command Summary

| Command | Purpose |
|---------|---------|
| `git init` | Initialize a repository |
| `git status` | Display repository status |
| `git add` | Stage files |
| `git commit` | Create a snapshot |
| `git log` | Show commit history |

---

# Lesson Checklist

Before moving on, make sure you can:

- [ ] Initialize a Git repository.
- [ ] Explain what `git init` creates.
- [ ] Stage files correctly.
- [ ] Create a meaningful commit.
- [ ] View commit history.
- [ ] Explain the Working Directory → Staging Area → Repository workflow.

---

# What's Next?

Congratulations!

You have completed **Module 1 – Git Fundamentals**.

In Module 2, you'll begin using Git daily and learn the commands that software engineers use every day.

---

⬅️ Previous: [Git Configuration](07-Configuring-Git.md)

