# Scenario 003 - Commit on the Wrong Branch

## Scenario
You accidentally committed changes on main instead of a feature branch.

## Solution
```bash
git branch feature-auth
git reset --hard HEAD~1
git switch feature-auth
```

## Explanation
Move the work to a feature branch and remove it from main.

## Interview Follow-up
What if the commit was already pushed?