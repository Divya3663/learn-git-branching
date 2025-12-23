# Learn git branching:
Git branching means creating a separate line of work so you can try new ideas without breaking your main project.
# Level-1 [git commit]
A Git commit is saving your code changes with a message so you can track and return to them later.
<img width="1919" height="803" alt="Screenshot 2025-12-22 145334" src="https://github.com/user-attachments/assets/f0b703d9-da61-4a58-813e-d410eab92151" />
A Git commit is saving your code changes with a message so you can track and return to them later.Command ```git commit```.
# Level-1 [git branches]
Git branches are separate paths in Git that let you work on features or fixes without affecting the main code.
<img width="1919" height="796" alt="Screenshot 2025-12-22 145953" src="https://github.com/user-attachments/assets/b9554722-b42b-4cf5-be35-dc7ec23d233f" />
This step shows creating a new branch called bugFix and switching to it, so now both main and bugFix point to the same commit, but bugFix is the active branch where new work will happen.Command ```git checkout -b bugFix```.
# level-1 [Branches and Merging]
Branches let you work on new features or fixes separately from the main code, and merging means combining those changes back into the main branch once the work is complete.
<img width="1916" height="804" alt="Screenshot 2025-12-22 150631" src="https://github.com/user-attachments/assets/fe4acb2f-3f63-4c53-80fa-539a75a22695" />
Commands to be Execute:
  ```
git checkout -b bugFix
 git commit
 git checkout main
 git commit
 git merge bugfix
```
# Level-1 [Git Rebase]
Git rebase moves your branch commits onto another branch to make the history clean and straight.
<img width="1919" height="797" alt="Screenshot 2025-12-22 151204" src="https://github.com/user-attachments/assets/cd393807-dfaf-4354-a198-1bfdca634459" />
Commands to be Executed:
 ```
git checkout -b bugFix
 git commit
 git checkout main
 git commit
 git checkout bugFix
 git rebase main
```
# Level-2 [Moving around in git]
Moving around in Git means navigating between commits and branches to see or work on different versions of your code using commands like checkout and switch in Git.
<img width="1919" height="799" alt="Screenshot 2025-12-22 192457" src="https://github.com/user-attachments/assets/7bc2adf2-4b38-4688-872c-653219b20059" />
In this level, HEAD is detached by using git checkout C4. Usually, HEAD points to a branch like main or bugFix. When you checkout a commit directly, HEAD moves to that commit and is not linked to any branch. The branches stay where they are, and you just view an older version of the project without changing branch history.Command ```git checkout C4```.

# Level-2 [Relative Refs]
Relative refs in Git let you move to commits based on their position from HEAD, instead of using full commit IDs, like HEAD~1 (one commit before HEAD) or HEAD^ (parent commit).
<img width="1919" height="797" alt="Screenshot 2025-12-22 193037" src="https://github.com/user-attachments/assets/a8418f12-8d32-42d6-910e-82e5aa5908a0" />
In this level, relative references are used to move HEAD to a parent commit instead of typing the full commit ID. The caret symbol ^ means “go to the parent commit.” When you use a command like git checkout C3 (or HEAD^), HEAD moves one step up in the commit history. This makes it easy to navigate to earlier commits quickly and safely without changing any branch positions.Command```git checkout C3```.
# Level-2 [Relative Refs 2(~)]
Relative Refs (~) are used to move back multiple commits from HEAD, for example HEAD~2 moves two commits back.
<img width="1918" height="806" alt="Screenshot 2025-12-22 194350" src="https://github.com/user-attachments/assets/2088e59c-c5f4-47f1-b307-8ef59a07992e" />
Commands to be Executed:
 ```
git branch -f main C6
 git branch -f bugFix HEAD~2
 git checkout C1
```
# Level-2 [Reversing Changes in Git]
Reversing changes in Git means undoing commits or file changes to return your project to an earlier, correct state using commands like git restore, git reset, or git revert.
<img width="1919" height="795" alt="Screenshot 2025-12-22 194755" src="https://github.com/user-attachments/assets/005bc443-0b73-4c8a-af35-1c9232daa9ac" />
Commands to be Executed:
```
git branch -f loacl C1
 git checkout pushed
 git revert pushed
```

# Level-3 [Moving Work Around]
Moving Work Around in Git means rearranging commits between branches using commands like cherry-pick or rebase to place your work where it belongs.
<img width="1919" height="799" alt="Screenshot 2025-12-22 195257" src="https://github.com/user-attachments/assets/695b37f8-a515-4f08-aec8-fb433b1e5a06" />
n this level, moving work around is done using git cherry-pick. Cherry-pick allows you to copy specific commits from different branches and apply them to the current branch. Here, the command ```git cherry-pick C3 C4 C7 ```takes the changes from commits C3, C4, and C7 and applies them one by one onto the main branch. This is useful when you want only selected changes, not the entire branch history.
# Level-3 [Git Interactive Rebase]
A Git feature that allows you to edit, reorder, combine, or remove commits in a branch’s history, enabling a cleaner and more organized commit structure before merging.
<img width="1919" height="800" alt="Screenshot 2025-12-22 203125" src="https://github.com/user-attachments/assets/9ed0fc31-7d1f-4f22-a872-2f0d3153b1ad" />
Commands to be Executed:
 ```
git rebase -i HEAD~4
 git branch -f main C5
 git rebase -i HEAD~4
 git branch -f overHere C5'
 git rebase overHere
```

# Level-4 [Locally stacked commits]
Locally stacked commits means you have created multiple commits one after another on your local branch, and these commits exist only on your local machine because they have not been pushed to a remote repository yet.
<img width="1919" height="798" alt="Screenshot 2025-12-23 111543" src="https://github.com/user-attachments/assets/bf597fba-ed17-43b2-b5a3-acba5581ee8a" />
Commands to be Executed:
```
git rebase -i HEAD~3
git checkout main
git branch -f main C4'
```











