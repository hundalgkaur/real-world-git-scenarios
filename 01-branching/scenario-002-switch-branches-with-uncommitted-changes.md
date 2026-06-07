# Scenario 002 - Switch Branches with Uncommitted Changes

## Scenario
You have local changes but need to move to another branch immediately.

## Solution
```bash
git stash
git switch bugfix-login
```

## Explanation
Stash temporarily saves your changes so you can switch safely.

## Interview Follow-up
What is the difference between stash apply and stash pop?