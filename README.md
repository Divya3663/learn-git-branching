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
1. git checkout -b bugFix
2. git commit
3. git checkout main
4. git commit
5. git merge bugfix
# Level-1 [Git Rebase]
Git rebase moves your branch commits onto another branch to make the history clean and straight.
<img width="1919" height="797" alt="Screenshot 2025-12-22 151204" src="https://github.com/user-attachments/assets/cd393807-dfaf-4354-a198-1bfdca634459" />
Commands to be Executed:
1.git checkout -b bugFix
2.git commit
3.git checkout main
4.git commit
5.git checkout bugFix
git rebase main





