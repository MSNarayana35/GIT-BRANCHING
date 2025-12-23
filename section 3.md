SECTION 3
Learn Git Branching – Cherry-pick Intro

Level 1

This level demonstrates how to use **`git cherry-pick`** to apply specific commits from different branches onto the current branch without merging the entire branch history
Cherry-picking allows selectively copying individual commits, which is useful when only certain changes (such as bug fixes or features) are needed from another branch without bringing unrelated commits.

<img width="1900" height="914" alt="Screenshot 2025-12-23 215315" src="https://github.com/user-attachments/assets/07536fb6-9fd5-4ecc-bbe9-1270601f667e" />


```bash
git cherry-pick c3 c4 c7
```
