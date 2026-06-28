# Installing Git

**Estimated Reading Time:** 10–15 minutes

---

# 💡 Did You Know?

Git is available on Windows, macOS, and Linux, making it one of the most widely supported developer tools.

Most modern development environments either include Git or provide an easy way to install it.

---

# Learning Objectives

By the end of this lesson, you will:

* Understand how to install Git on different operating systems.
* Verify that Git is installed correctly.
* Check the installed Git version.
* Understand why keeping Git updated is important.

---

# Why Do We Need to Install Git?

Git is a command-line application that runs on your local computer.

Before you can track changes, create commits, or collaborate with others, Git must be installed and available from your terminal.

---

# Installing Git

## macOS

Using Homebrew (recommended):

```bash
brew install git
```

Verify the installation:

```bash
git --version
```

---

## Windows

1. Download Git from the official website.
2. Run the installer.
3. Keep the default installation options if you're unsure.
4. Open **Git Bash** or **PowerShell**.

Verify:

```bash
git --version
```

---

## Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install git
```

Verify:

```bash
git --version
```

---

# Expected Output

Example:

```text
git version 2.51.0
```

> Your version may be different depending on when you install Git.

---

# Updating Git

Keeping Git updated gives you:

* Bug fixes
* Performance improvements
* New features
* Security updates

How you update Git depends on your operating system and package manager.

For example, on macOS with Homebrew:

```bash
brew update
brew upgrade git
```

---

# Verify Your Installation

Run the following commands:

```bash
which git
git --version
git --help
```

On Windows, replace `which` with:

```bash
where git
```

These commands confirm:

* Where Git is installed
* Which version is installed
* That Git is functioning correctly

---

# Real-World Example

Imagine you join a new company.

One of your first setup tasks is installing development tools:

* Git
* VS Code
* Java
* Docker
* Kubernetes CLI (kubectl)

Git is usually the first tool configured because almost every project depends on it.

---

# Hands-on Lab

Complete the following:

1. Install Git.
2. Verify the version.
3. Locate the Git executable.
4. Open the Git help page.
5. Record your Git version.

---

# Common Mistakes

❌ Forgetting to verify the installation.

❌ Using an outdated Git version for a new project.

❌ Installing Git but not adding it to the system PATH (common on Windows).

---

# Interview Questions

### Beginner

* How do you verify that Git is installed?
* Which command shows the installed Git version?

### Intermediate

* Why should you keep Git updated?
* How would you install Git on Linux?

---

# Key Takeaways

* Git must be installed before you can use it.
* Always verify the installation.
* Learn how to locate the Git executable.
* Keep Git updated to benefit from improvements.

---

# What's Next?

In the next lesson, you'll configure Git with your identity and understand the difference between **system**, **global**, and **local** Git configuration.

---

⬅️ Previous: [Git Architecture](05-Git-Architecture.md)

➡️ Next: [Git Configuration](07-Configuring-Git.md)
