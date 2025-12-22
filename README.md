# Learn git branching:
Git branching means creating a separate line of work so you can try new ideas without breaking your main project.
# Level-1 [git commit]
A Git commit is saving your code changes with a message so you can track and return to them later.
<img width="1919" height="803" alt="Screenshot 2025-12-22 145334" src="https://github.com/user-attachments/assets/f0b703d9-da61-4a58-813e-d410eab92151" />
A Git commit is saving your code changes with a message so you can track and return to them later.Command '''git commit'''.
# Level-2 [git branches]
Git branches are separate paths in Git that let you work on features or fixes without affecting the main code.
<img width="1919" height="796" alt="Screenshot 2025-12-22 145953" src="https://github.com/user-attachments/assets/b9554722-b42b-4cf5-be35-dc7ec23d233f" />
This step shows creating a new branch called bugFix and switching to it, so now both main and bugFix point to the same commit, but bugFix is the active branch where new work will happen.Command '''git checkout -b bugFix'''.
# level-1 [Branches and Merging]
Branches let you work on new features or fixes separately from the main code, and merging means combining those changes back into the main branch once the work is complete.
<img width="1916" height="804" alt="Screenshot 2025-12-22 150631" src="https://github.com/user-attachments/assets/fe4acb2f-3f63-4c53-80fa-539a75a22695" />
Commands to be Execute:
1. ```git checkout -b bugFix
2. git commit
3. git checkout main
4. git commit
5. git merge bugfix```
# Level-1 [Git Rebase]
Git rebase moves your branch commits onto another branch to make the history clean and straight.
<img width="1919" height="797" alt="Screenshot 2025-12-22 151204" src="https://github.com/user-attachments/assets/cd393807-dfaf-4354-a198-1bfdca634459" />
Commands to be Executed:
1. ```git checkout -b bugFix
2. git commit
3. git checkout main
4. git commit
5. git checkout bugFix
6. git rebase main```
# Level-2 [Moving around in git]
Moving around in Git means navigating between commits and branches to see or work on different versions of your code using commands like checkout and switch in Git.
<img width="1919" height="799" alt="Screenshot 2025-12-22 192457" src="https://github.com/user-attachments/assets/7bc2adf2-4b38-4688-872c-653219b20059" />
In this level, HEAD is detached by using git checkout C4. Usually, HEAD points to a branch like main or bugFix. When you checkout a commit directly, HEAD moves to that commit and is not linked to any branch. The branches stay where they are, and you just view an older version of the project without changing branch history.Command '''git checkout C4'''.

# Level-2 [Relative Refs]
Relative refs in Git let you move to commits based on their position from HEAD, instead of using full commit IDs, like HEAD~1 (one commit before HEAD) or HEAD^ (parent commit).
<img width="1919" height="797" alt="Screenshot 2025-12-22 193037" src="https://github.com/user-attachments/assets/a8418f12-8d32-42d6-910e-82e5aa5908a0" />
In this level, relative references are used to move HEAD to a parent commit instead of typing the full commit ID. The caret symbol ^ means “go to the parent commit.” When you use a command like git checkout C3 (or HEAD^), HEAD moves one step up in the commit history. This makes it easy to navigate to earlier commits quickly and safely without changing any branch positions.Command'''git checkout C3'''.
# Level-2 [Relative Refs #2(~)]
Relative Refs (~) are used to move back multiple commits from HEAD, for example HEAD~2 moves two commits back.
<img width="1918" height="806" alt="Screenshot 2025-12-22 194350" src="https://github.com/user-attachments/assets/2088e59c-c5f4-47f1-b307-8ef59a07992e" />

Commands to be Executed:
1. ```git branch -f main C6
2. git branch -f bugFix HEAD~2
3. git checkout C1```






