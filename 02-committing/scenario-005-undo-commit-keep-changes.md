# Scenario 005 - Undo Commit but Keep Changes

## Scenario
You committed too early and want to modify the changes before recommitting.

## Solution
```bash
git reset --soft HEAD~1
```

## Explanation
Removes the commit but keeps all changes staged.

## Interview Follow-up
What is the difference between --soft, --mixed and --hard?