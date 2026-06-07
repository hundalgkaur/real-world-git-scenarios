# Scenario 01 - Save Work Before Switching Branches

## Scenario

You are working on a feature branch and have several uncommitted changes.

Suddenly, your team lead asks you to switch to another branch and fix a production bug.

What Git command should you use?

---

## Solution

```bash
git stash
git switch bugfix-production
```

---

## Explanation

`git stash` temporarily saves your uncommitted changes and restores a clean working directory.

This allows you to safely switch branches without losing work.

---

## Alternative Solution

```bash
git commit -m "WIP: unfinished feature"
git switch bugfix-production
```

A temporary commit can also be used when you want to save your progress in the repository history.

---

## Common Mistakes

❌ Trying to switch branches with conflicting uncommitted changes.

❌ Forgetting to restore stashed work later using:

```bash
git stash pop
```

---

## Interview Follow-up

Q: How do you see all stashes?

```bash
git stash list
```

Q: How do you apply a stash without removing it?

```bash
git stash apply
```

