SECTION 2

Level 1: Detach yo’ HEAD (rampup1)

In this level, the goal is to understand what a **detached HEAD** means in Git. Normally, HEAD points to a branch, but in this level, HEAD is moved directly to a specific commit instead of a branch. By checking out a commit hash, HEAD becomes detached while the branches remain unchanged. This helps in understanding how Git can inspect past commits without affecting branch pointers.
<img width="1899" height="912" alt="Screenshot 2025-12-23 210820" src="https://github.com/user-attachments/assets/c27048f1-6abe-4536-9cdf-b5483c8707f2" />



```bash
git checkout c4
```



Level 2: Relative References (^) (rampup2)

This level introduces **relative references** using the caret (`^`) operator. The caret is used to move to the **parent commit** of a given branch or commit. By checking out `bugFix^`, HEAD moves one commit behind the `bugFix` branch. This level helps in navigating commit history without using full commit hashes.

<img width="1919" height="905" alt="Screenshot 2025-12-23 211020" src="https://github.com/user-attachments/assets/d9920f1f-0c57-492a-9bf9-e1337f079ea4" />



```bash
git checkout bugFix^
```



Level 3: Relative References #2 (~) (rampup3)

In this level, the tilde (`~`) operator and **direct commit references** are used. The task involves force-moving branches to specific commits and then detaching HEAD to a particular commit. This level demonstrates how branches can be repositioned using `git branch -f` and how HEAD can be detached using a commit hash. It builds confidence in rewriting branch pointers safely in a controlled environment.

<img width="1905" height="900" alt="Screenshot 2025-12-23 211350" src="https://github.com/user-attachments/assets/d361ac51-ac46-4bc5-985c-cfe113e31ca7" />



```bash
git branch -f main c6
git branch -f bugFix c0
git checkout c1
```

Level 4: Reversing Changes in Git (Ramp Up 4)

This level focuses on understanding how **`git revert`** and **`git reset`** work, and how they differ when undoing changes in Git history.
In this level, I learned that git revert safely undoes a commit by creating a new commit, while git reset
--hard moves the branch pointer and discards commits, making revert safer for shared branches and reset more powerful but destructive,
with branch switching helping to isolate and control history changes.

<img width="1913" height="913" alt="Screenshot 2025-12-23 211744" src="https://github.com/user-attachments/assets/e3b800b4-fc5f-495b-9b37-a2463e719b52" />


```bash
git checkout pushed
git revert c2
git checkout local
git reset --hard c1
```
