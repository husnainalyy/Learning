
### GitHub Shortcuts

* = represents in which repo you are present

#### COLLABORATION

1. **Initialize a Git Repository**
   ```bash
   git init
   ```
   This command initializes a new Git repository. It creates a hidden `.git` directory in your project, where Git stores all the project’s metadata and object database.
   
   *Urdu:* Yeh command ek nayi Git repository initialize karta hai. Yeh aapke project mein ek chupi hui `.git` directory banata hai, jahan Git project ka sara metadata aur object database store karta hai.

2. **Add Files to Git**
   ```bash
   git add .
   ```
   This command adds all the files in the current directory to the staging area, making them ready for the next commit.
   
   *Urdu:* Yeh command current directory mein sabhi files ko staging area mein add kar deta hai, taki woh next commit ke liye tayar ho jayein.

3. **Commit the Files**
   ```bash
   git commit -m "message"
   ```
   This command commits the staged changes to the repository with a descriptive message. The `-m` flag allows you to add a commit message directly from the command line.
   
   *Urdu:* Yeh command staged changes ko repository mein commit karta hai aur ek descriptive message add karta hai. `-m` flag se aap command line se directly commit message de sakte hain.

4. **Rename the Branch to Main**
   ```bash
   git branch -M main
   ```
   This command renames the current branch to `main`. If a branch named `main` already exists, it will merge the current branch into `main`.
   
   *Urdu:* Yeh command current branch ka naam `main` rakhta hai. Agar `main` naam ki branch pehle se maujood hai, to yeh current branch ko `main` mein merge kar dega.

5. **Add the GitHub Repo**
   ```bash
   git remote add origin repo-link
   ```
   This command adds a remote repository link (usually from GitHub) to your local Git repository. The remote repository is usually referred to as `origin`.
   
   *Urdu:* Yeh command aapki local Git repository mein ek remote repository ka link (usually GitHub se) add karta hai. Remote repository ko aam tor par `origin` kaha jata hai.

6. **Push Files to GitHub**
   ```bash
   git push origin -u branchName
   ```
   This command pushes your commits to the remote repository on the specified branch. The `-u` flag sets the default remote and branch for future pushes.
   
   *Urdu:* Yeh command aapke commits ko specified branch par remote repository mein push karta hai. `-u` flag se future pushes ke liye default remote aur branch set ho jata hai.

---

7. **Clone a Repo**
   ```bash
   git clone repo-link
   ```
   This command creates a local copy of a remote repository. It downloads the repository from the given link and sets up everything locally.
   
   *Urdu:* Yeh command ek remote repository ka local copy banata hai. Yeh di gayi link se repository download karta hai aur sab kuch locally set up kar deta hai.

---

8. **Fetch Code from Repo**
   ```bash
   git fetch
   ```
   This command downloads new data from a remote repository without merging it into your local branch. It's useful for seeing what others have been working on.
   
   *Urdu:* Yeh command remote repository se naya data download karta hai bina usay aapki local branch mein merge kiye. Yeh dekhne ke liye useful hai ke doosre log kya kaam kar rahe hain.

9. **Fetch and Merge Code**
   ```bash
   git pull
   ```
   This command fetches new data from a remote repository and immediately merges it into your current branch. It's a combination of `git fetch` and `git merge`.
   
   *Urdu:* Yeh command remote repository se naya data fetch karta hai aur foran hi aapki current branch mein merge kar deta hai. Yeh `git fetch` aur `git merge` ka combination hai.

---

10. **Check File Status**
    ```bash
    git status -s
    ```
    This command shows the status of changes as a short summary. It tells you which files are staged, unstaged, and untracked.
    
    *Urdu:* Yeh command changes ka status short summary ke tor par dikhata hai. Yeh batata hai ke kaunsi files staged, unstaged, aur untracked hain.

11. **Check Commit History**
    ```bash
    git log
    ```
    This command shows the commit history of the current branch. It displays each commit's hash, author, date, and message.
    
    *Urdu:* Yeh command current branch ki commit history dikhata hai. Yeh har commit ka hash, author, date, aur message dikhata hai.

12. **Check Commit History (Simplified)**
    ```bash
    git log --oneline
    ```
    This command shows the commit history in a simplified, one-line-per-commit format.
    
    *Urdu:* Yeh command commit history ko simplified format mein dikhata hai, jahan har commit ek line mein hoti hai.

13. **Check Commit History with Graph**
    ```bash
    git log --oneline --graph
    ```
    This command shows the commit history in a simplified format with a graph showing branch and merge history.
    
    *Urdu:* Yeh command commit history ko simplified format mein dikhata hai, saath mein ek graph ke sath jo branch aur merge history dikhata hai.

---

14. **Move Back One Step**
    ```bash
    git reset --hard HEAD~1
    ```
    This command resets your current branch to the state it was one commit ago, discarding all changes.
    
    *Urdu:* Yeh command aapki current branch ko ek commit pehle ki state par reset kar deta hai, saare changes ko discard karte hue.

15. **Remove Git Initialization**
    ```powershell
    Remove-Item -Path .git -Recurse -Force
    ```
    This command removes the `.git` directory, effectively un-initializing the Git repository.
    
    *Urdu:* Yeh command `.git` directory ko remove karta hai, jisse Git repository un-initialize ho jati hai.

---

16. **Make a Branch**
    ```bash
    git branch name
    ```
    This command creates a new branch with the specified name.
    
    *Urdu:* Yeh command specified naam ke sath ek nayi branch banata hai.

17. **Switch to a Branch**
    ```bash
    git switch name
    ```
    This command switches to the branch with the specified name.
    
    *Urdu:* Yeh command specified naam wali branch par switch karta hai.

---

#### To Merge Two Branches

18. **Switch to Main Branch**
    ```bash
    git switch main
    ```
    This command switches to the `main` branch.
    
    *Urdu:* Yeh command `main` branch par switch karta hai.

19. **Merge with Another Branch**
    ```bash
    git merge name
    ```
    This command merges the specified branch into the current branch.
    
    *Urdu:* Yeh command specified branch ko current branch mein merge karta hai.

---

#### Handling Merge Conflicts

- **Accept Current Change:**
  Accept the changes from your current branch.
  *Urdu:* Current branch ka code accept karna.
  
- **Accept Incoming Change:**
  Accept the changes from the branch being merged.
  *Urdu:* Merge hone wali branch ka code accept karna.
  
- **Accept Both Changes:**
  Accept both changes, keeping both versions.
  *Urdu:* Dono branches ka code accept karna.
  
- **Compare Changes:**
  Compare the changes from both branches.
  *Urdu:* Dono branches ke code ko compare karna.

---

#### Delete Branch

20. **Delete a Branch**
    ```bash
    git branch -d name
    ```
    This command deletes the specified branch.
    
    *Urdu:* Yeh command specified branch ko delete karta hai.

---

#### Stash Changes

21. **Stash Changes**
    ```bash
    git stash
    ```
    This command temporarily saves your changes, allowing you to switch branches without committing.
    
    *Urdu:* Yeh command aapke changes ko temporarily save karta hai, taki aap bina commit kiye branch switch kar sakein.

22. **Apply Stashed Changes**
    ```bash
    git stash apply
    ```
    This command applies the stashed changes back to your working directory.
    
    *Urdu:* Yeh command stashed changes ko wapas aapki working directory mein apply karta hai.

23. **Clear Stash**
    ```bash
    git stash clear
    ```
    This command removes all stashed entries.
    
    *Urdu:* Yeh command saari stashed entries ko remove kar deta hai.

---

This detailed guide covers each Git command with a clear explanation in both English and Urdu to help anyone understand and use these commands effectively.







-------------------------- git hub shortcuts -------------------------------
* represent in which repo you are present


git init   ==> initialize the git
git add .  ==> add the files to git
git commit -m "message"   ==>  commit the files
git branch -M main  ==> it will forcefully rename the switched branch to main if main is present it merge both these branches into one
git remote add origin repo-link   ==>  add the  github repo
git push origin -u branchName   ==>  send files to github


git clone link-repo  ==> you can clone the code 


git fetch  ==> you can fetch the code which is added in the repo

git pull   ==> fetch and merge in one step





git status -s   told us that files are change or its status and it done befor commit or after commit
if we want to get all history we write git log but if we want the name or time then
git log --oneline   ==> to check all the commits histories
git log --oneline --graph  ==> can give the path

git reset --hard HEAD~1  ==>  to move back one step if we write 2 affter head it moves two step4s
Remove-Item -Path .git -Recurse -Force ==> To remove a Git repository initialization from a project,


git branch name   ==> make a branch 
git switch name   ==> switch to that branch which has name


to merge the two branches

git switch main   ==> you should be switched to main branch
git merge name    ==> jis branch k sath merge krna chahty ho us ka name likh do 


if you want to merge two branches same file which has different code at same line let see line 3 has different code then CONFLICT IS HAPPEN you can solve it by clicking

accept current change
accept incoming change
accept both changes
compare changes



DELETE BRANCH 

git branch -d name    ==>you can delete a branch by giving name of that branch



git stash  ==>if you move to other branch but you not commit it then it delete so you stash it (aap code ko draft my rkh dety ho    ) then if you come back or took those changes you just type

git stash apply   ==> to get the stash code 

git stash clear    ==> if you want to delete stashh code 



COLLABORATION 
