Level 1

In this level, I learned that a commit is used to save changes in Git. Each commit creates a new version of the project, and by making multiple commits, Git builds the complete history of the project over time.

<img width="1915" height="908" alt="Screenshot 2025-12-22 221924" src="https://github.com/user-attachments/assets/5142ff15-5926-4845-9a10-b50baa5f03d7" />


```bash
git commit
git commit
```

Level 2

In this level, I learned that a branch allows developers to work on a new feature separately without affecting the main code. I created a new branch named bugFix and switched to it to work independently.

<img width="1897" height="910" alt="Screenshot 2025-12-22 222457" src="https://github.com/user-attachments/assets/52c5a8a7-2c3a-4d33-bfad-380bb80d18b6" />


```bash
git branch bugFix
git checkout bugFix
```



Level 3

In this level, I learned how to merge changes from one branch into another. I first made a commit in the bugFix branch, then made a commit in the main branch, and finally merged the bugFix branch into main, which created a merge commit.

<img width="1898" height="911" alt="Screenshot 2025-12-22 222810" src="https://github.com/user-attachments/assets/a4594792-bda8-486b-b7ae-42fb791c3d38" />


```bash
git checkout -b bugFix
git commit
git checkout main
git commit
git merge bugFix
```


Level 4

In this level, I learned that rebase is used to move commits from one branch on top of another branch to maintain a clean and linear commit history. I committed changes in the bugFix branch and then rebased it onto the main branch.

<img width="1886" height="905" alt="Screenshot 2025-12-22 223002" src="https://github.com/user-attachments/assets/dc3f9d4c-ae6e-4c4a-a8f2-f397f0ad370c" />


```bash
git checkout -b bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```


