SECTION 3
Learn Git Branching – Cherry-pick Intro

Level 1

This level demonstrates how to use **`git cherry-pick`** to apply specific commits from different branches onto the current branch without merging the entire branch history
Cherry-picking allows selectively copying individual commits, which is useful when only certain changes (such as bug fixes or features) are needed from another branch without bringing unrelated commits.

<img width="1900" height="914" alt="Screenshot 2025-12-23 215315" src="https://github.com/user-attachments/assets/07536fb6-9fd5-4ecc-bbe9-1270601f667e" />


```bash
git cherry-pick c3 c4 c7
```


Level 2

This level demonstrates how to use **interactive rebase** to modify recent commit history in a controlled way.

Using **`git rebase -i`**, we can reorder, edit, squash, or remove commits by specifying a target commit using **relative references** like `HEAD~n`. This is especially useful for cleaning up commit history before sharing changes.

In this level, interactive rebase is performed on the last few commits to rearrange or adjust them to match the goal state.

<img width="1899" height="908" alt="Screenshot 2025-12-23 224445" src="https://github.com/user-attachments/assets/5e72f32c-28ce-4d0e-849a-88df0f20bfe4" />


```bash
git rebase -i HEAD~4
```
