# All_git_commands-

# Git Commands for Developers 

Yeh document un Git commands ko explain karta hai jo aapko ek Git repository ko manage karne ke liye zaroori hoti hain. Yeh commands daily development work ke liye kaafi useful hain.

## Basic Git Commands

### 1. `git init`
- **Usage**: `git init`
- **Description**: Ye command ek naya Git repository initialize karta hai current directory mein. Isse ek `.git` folder create hota hai jo repository ke saare configurations rakhta hai.

### 2. `git clone <repository-url>`
- **Usage**: `git clone https://github.com/username/repository.git`
- **Description**: Ye command ek remote repository ko local machine par clone karta hai, jisse aap apna kaam start kar sakte hain.

### 3. `git status`
- **Usage**: `git status`
- **Description**: Ye command repository ka status dikhata hai, jaise ki kaunse files modified hain, kaunse files staged hain, aur kaunse files untracked hain.

### 4. `git add <file>`
- **Usage**: `git add index.html`
- **Description**: Ye command specific file ko staging area mein add karta hai, taaki wo file commit ke liye ready ho sake.

### 5. `git commit -m "message"`
- **Usage**: `git commit -m "Initial commit"`
- **Description**: Ye command staged changes ko commit karta hai, aur aapko ek commit message dena padta hai.

### 6. `git log`
- **Usage**: `git log`
- **Description**: Ye command aapko commit history dikhata hai, jisme commit hashes, authors, dates, aur messages shamil hote hain.

### 7. `git diff`
- **Usage**: `git diff`
- **Description**: Ye command working directory aur staging area ke beech differences dikhata hai. Matlab, aapne jo changes kiye hain unhe compare karta hai.

### 8. `git reset <file>`
- **Usage**: `git reset index.html`
- **Description**: Ye command ek file ko unstage kar deta hai. Matlab, file staging area se hata di jaati hai lekin working directory mein changes rehte hain.

## Branching Commands

### 9. `git branch`
- **Usage**: `git branch`
- **Description**: Ye command aapko current repository mein saare branches dikhata hai. Jo branch active hota hai, wo highlight hota hai.

### 10. `git branch <branch-name>`
- **Usage**: `git branch feature-xyz`
- **Description**: Ye command ek naya branch create karta hai, lekin aap is branch pe switch nahi karte.

### 11. `git checkout <branch-name>`
- **Usage**: `git checkout feature-xyz`
- **Description**: Ye command aapko specific branch pe switch karne ke liye use hoti hai.

### 12. `git checkout -b <branch-name>`
- **Usage**: `git checkout -b feature-xyz`
- **Description**: Ye command ek naya branch create karta hai aur turant us branch pe switch kar leta hai.

### 13. `git merge <branch-name>`
- **Usage**: `git merge feature-xyz`
- **Description**: Ye command specified branch ko current branch mein merge kar deti hai.

### 14. `git branch -d <branch-name>`
- **Usage**: `git branch -d feature-xyz`
- **Description**: Ye command ek branch ko delete kar deti hai, jab wo merge ho chuka hota hai.

## Remote Repository Commands

### 15. `git remote add origin <repository-url>`
- **Usage**: `git remote add origin https://github.com/username/repository.git`
- **Description**: Ye command remote repository URL ko aapke local repository se connect karta hai, taaki aap changes push ya pull kar sakein.

### 16. `git push -u origin <branch-name>`
- **Usage**: `git push -u origin main`
- **Description**: Ye command aapke local branch ko remote repository pe push karta hai aur upstream branch set kar deta hai.

### 17. `git pull origin <branch-name>`
- **Usage**: `git pull origin main`
- **Description**: Ye command remote repository se changes fetch karta hai aur unhe aapke current branch mein merge karta hai.

### 18. `git fetch`
- **Usage**: `git fetch`
- **Description**: Ye command remote repository se changes fetch karta hai lekin unhe merge nahi karta. Aap pehle changes ko review kar sakte ho.

### 19. `git push origin --delete <branch-name>`
- **Usage**: `git push origin --delete feature-xyz`
- **Description**: Ye command remote repository se specified branch ko delete kar deta hai.

## Stashing Commands

### 20. `git stash`
- **Usage**: `git stash`
- **Description**: Ye command aapke current changes ko temporarily stash kar leta hai, taaki aap bina commit kiye dusra kaam kar sakein.

### 21. `git stash pop`
- **Usage**: `git stash pop`
- **Description**: Ye command sabse recent stash ko wapas apply kar deta hai aur stash list se usse remove kar deta hai.

### 22. `git stash list`
- **Usage**: `git stash list`
- **Description**: Ye command stash ki list dikhata hai, jo aapne save ki hui hoti hai.

### 23. `git stash drop`
- **Usage**: `git stash drop`
- **Description**: Ye command stash ko list se hata deta hai.

## Git Configuration Commands

### 24. `git config --global user.name "Your Name"`
- **Usage**: `git config --global user.name "John Doe"`
- **Description**: Ye command aapka Git user name globally set karta hai.

### 25. `git config --global user.email "your-email@example.com"`
- **Usage**: `git config --global user.email "john.doe@example.com"`
- **Description**: Ye command aapka email globally set karta hai Git commits ke liye.

## Viewing and Comparing Commands

### 26. `git show <commit-hash>`
- **Usage**: `git show abc1234`
- **Description**: Ye command ek specific commit ka detailed information dikhata hai, jaise changes aur commit message.

### 27. `git diff <commit-hash> <commit-hash>`
- **Usage**: `git diff abc1234 def5678`
- **Description**: Ye command do commits ke beech differences dikhata hai.

### 28. `git blame <file>`
- **Usage**: `git blame index.html`
- **Description**: Ye command file ke har line ka author dikhata hai, jo last modify ki thi.

## Undoing Changes

### 29. `git revert <commit-hash>`
- **Usage**: `git revert abc1234`
- **Description**: Ye command ek commit ko revert kar deta hai, jo new commit banata hai aur previous commit ke changes ko undo karta hai.

### 30. `git rm <file>`
- **Usage**: `git rm oldfile.txt`
- **Description**: Ye command file ko working directory aur staging area se remove kar deta hai.

### 31. `git reset --hard`
- **Usage**: `git reset --hard`
- **Description**: Ye command current branch ko last commit pe reset kar deta hai aur saare local changes discard kar deta hai.

---
