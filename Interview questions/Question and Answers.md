
---

### **1. You committed the wrong file by mistake. How will you remove it?**

👉 Use:

```bash
git reset HEAD~1   # undo last commit, keep changes
git rm filename
git commit -m "removed wrong file"
```

✅ Explain: *“I’ll reset or revert the commit and remove the file properly.”*

---

### **2. You pushed a bad commit to GitHub. How will you fix it safely?**

👉 Use:

```bash
git revert <commit-id>
git push origin master
```

✅ Explain: *“I’ll use `git revert` to create a new commit that undoes the bad commit, so history is safe.”*

---

### **3. How do you undo the last commit but keep the changes in working directory?**

👉 Use:

```bash
git reset --soft HEAD~1
```

✅ Explain: *“This removes the commit but keeps my changes staged so I can recommit correctly.”*

---

### **4. Your teammate pushed code, how do you update your local repo?**

👉 Use:

```bash
git pull origin master
```

✅ Explain: *“I’ll pull the latest changes from remote to keep my local repo up-to-date.”*

---

### **5. You want to see what files changed in the last commit.**

👉 Use:

```bash
git show --pretty="" --name-only
```

✅ Explain: *“This shows me only the file names that changed in the last commit.”*

---

### **6. You want to work on a new feature without disturbing `master`.**

👉 Use:

```bash
git checkout -b feature/login
```

✅ Explain: *“I’ll create a new branch for my feature, so master stays clean.”*

---

### **7. How do you delete a file from Git but keep it locally?**

👉 Use:

```bash
git rm --cached filename
git commit -m "removed file from tracking"
```

✅ Explain: *“`--cached` removes it from Git but keeps it in my working directory.”*

---

### **8. You accidentally staged a file with `git add`. How do you unstage it?**

👉 Use:

```bash
git reset HEAD filename
```

✅ Explain: *“I’ll use reset to remove the file from staging, but it will stay in my working directory.”*

---

### **9. How do you ignore sensitive files like `.env` in Git?**

👉 Use:

* Add file to `.gitignore`:

  ```
  .env
  ```

✅ Explain: *“I’ll add it to `.gitignore` so Git never tracks it.”*

---

### **10. You want to check the remote URL your repo is connected to.**

👉 Use:

```bash
git remote -v
```

✅ Explain: *“This shows me the fetch and push URLs for my remote repo.”*

---
