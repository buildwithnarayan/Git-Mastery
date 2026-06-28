# Configuring Git

**Estimated Reading Time:** 15–20 minutes

---

# 💡 Did You Know?

Every Git commit records the **author's name** and **email address**. Git uses your configuration to populate this information automatically.

Without proper configuration, your commits may be attributed to the wrong identity.

---

# Learning Objectives

By the end of this lesson, you will:

- Configure your Git identity.
- Understand system, global, and local configuration.
- View and edit Git configuration.
- Verify your configuration.
- Learn best practices for managing Git settings.

---

# Why Configure Git?

Before creating commits, Git needs to know:

- Who created the commit?
- Which email address should be associated with it?

This information becomes part of every commit.

---

# Configuration Levels

Git supports three configuration levels.

## 1. System Configuration

Applies to every user on the computer.

```bash
git config --system
```

Usually managed by system administrators.

---

## 2. Global Configuration

Applies to the current user.

```bash
git config --global
```

This is the configuration you'll use most often.

---

## 3. Local Configuration

Applies only to the current repository.

```bash
git config --local
```

Useful when you need a different identity for a specific project.

---

# Configure Your Identity

Set your name:

```bash
git config --global user.name "Narayan Prasad"
```

Set your email:

```bash
git config --global user.email "your-email@example.com"
```

Replace the email with the one associated with your Git hosting account (for example, GitHub).

---

# Verify Your Configuration

View all settings:

```bash
git config --list
```

View your name:

```bash
git config user.name
```

View your email:

```bash
git config user.email
```

---

# Where Is the Configuration Stored?

On macOS and Linux, global configuration is typically stored in:

```text
~/.gitconfig
```

Local configuration is stored in:

```text
.git/config
```

Open the global configuration:

```bash
cat ~/.gitconfig
```

---

# Edit Configuration

Open the global configuration in your default editor:

```bash
git config --global --edit
```

---

# Local Configuration Example

Imagine you're contributing to an open-source project using a personal email, but your office repositories use your company email.

Inside the project:

```bash
git config --local user.email "personal@example.com"
```

This change affects only that repository.

---

# Industry Insight

Many developers have:

- A personal GitHub account.
- A company Git hosting account.

Using local configuration allows them to use different identities for different repositories.

---

# Hands-on Lab

1. Configure your global name.
2. Configure your global email.
3. Verify the configuration.
4. Open `~/.gitconfig`.
5. Create a test repository and set a different local email.
6. Compare the global and local configurations.

---

# Common Mistakes

❌ Forgetting to configure Git before the first commit.

❌ Using a work email in personal repositories.

❌ Assuming local configuration changes the global configuration.

---

# Interview Questions

### Beginner

- Which command sets your Git username?
- Where is the global Git configuration stored?

### Intermediate

- What is the difference between global and local configuration?
- How do you display all Git configuration values?

### Advanced

- Which configuration level takes precedence if the same setting exists in system, global, and local configurations?
- When would you use local configuration in a real project?

---

# Command Summary

| Command | Purpose |
|----------|---------|
| `git config --global user.name` | Set global username |
| `git config --global user.email` | Set global email |
| `git config --list` | Show all configuration |
| `git config --global --edit` | Edit global configuration |
| `git config --local user.email` | Override email for one repository |

---

# Key Takeaways

- Git records your identity with every commit.
- Global configuration applies to all repositories for your user.
- Local configuration overrides global settings for a specific repository.
- Always verify your configuration before contributing to a project.

---

# What's Next?

In the next lesson, you'll create your first Git repository, make your first commit, and inspect the `.git` directory to understand exactly what Git creates behind the scenes.

---

⬅️ Previous: [Git Installation](06-Installing-Git.md)

➡️ Next: [Your First Git Repository](08-Your-First-Git-Repository.md)
