# Scenario 001 - Create a Feature Branch

## Real-World Scenario
Imagine your team has a shopping application. The `main` branch contains the stable version used by customers.

Your manager asks you to add a new Login feature.

Should you directly start coding on `main`?

No. If you make mistakes, you could break the stable version used by everyone.

Instead, create a separate branch for your work.

---

## Solution

```bash
git switch -c feature-authentication
```

---

## What Happens Behind the Scenes?

Think of Git branches like copies of a school notebook.

- The original notebook = `main`
- Your personal notebook = `feature-authentication`

You can write, erase, experiment, and make mistakes in your notebook without affecting the original one.

---

## Step-by-Step Explanation

### Step 1

```bash
git switch -c feature-authentication
```

Git does two things:

1. Creates a new branch called `feature-authentication`
2. Moves you to that branch immediately

---

### Step 2

Make your code changes.

Example:

- Add login screen
- Add API calls
- Add validation

---

### Step 3

Commit your work.

```bash
git add .
git commit -m "Add authentication feature"
```

---

### Step 4

Merge the branch after testing.

```bash
git switch main
git merge feature-authentication
```

---

## Explain Like I'm 10

Imagine your teacher gives the class a clean drawing.

Instead of drawing directly on the original paper, you make a photocopy and practice on it.

If you make mistakes, the original drawing is still safe.

A Git branch works exactly the same way.

---

## Common Mistakes

❌ Working directly on `main`

❌ Creating unclear branch names such as:

```text
new-feature
work1
changes
```

✅ Better names:

```text
feature-login
feature-authentication
bugfix-payment-error
```

---

## Interview Question

Q: Why do developers create feature branches?

Answer:

Feature branches isolate changes, protect the main branch, support teamwork, and make code reviews easier.

---

## Key Takeaway

Never start a new feature directly on `main`.

Create a feature branch first so your work stays isolated, organized, and safe.