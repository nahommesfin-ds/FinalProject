# 🚀 GitHub Setup Guide for FinalProject

This guide will walk you through setting up your **FinalProject** repository on GitHub and pushing your code online.

---

## ✅ Pre-requisites

- [Git](https://git-scm.com/) installed on your system
- A [GitHub](https://github.com) account
- Your project files ready in `c:\pubh1142\`

### Files You Should Have:
✓ `FinalProject.ipynb` - Your main analysis notebook  
✓ `FINALPROJECT_README.md` - Comprehensive project README  
✓ `requirements.txt` - Python dependencies  
✓ `.gitignore` - Ignore patterns  

---

## 📋 Step 1: Create Repository on GitHub

### 1.1 Go to GitHub
- Visit [github.com](https://github.com) and sign in

### 1.2 Create New Repository
- Click the **+** icon in top-right → **New repository**
- **Repository name**: `FinalProject`
- **Description**: "A comprehensive data science analysis of occupational stress, lifestyle factors, and sleep quality"
- **Visibility**: Public (so others can see your work!)
- **Initialize with**: Do NOT check any boxes (we'll push existing code)
- Click **Create repository**

### 1.3 Copy Repository URL
You'll be taken to a page. Copy the HTTPS URL:
```
https://github.com/nahommesfin-ds/FinalProject.git
```

---

## 💻 Step 2: Set Up Git Locally

Open **PowerShell** or **Command Prompt** and navigate to your project:

```powershell
cd C:\pubh1142
```

### 2.1 Initialize Git Repository
```powershell
git init
```

### 2.2 Configure Git (First Time Only)
```powershell
git config --global user.name "Nahom Mesfin"
git config --global user.email "your.email@example.com"
```

### 2.3 Add Remote Repository
Replace with your actual URL:
```powershell
git remote add origin https://github.com/nahommesfin-ds/FinalProject.git
```

### 2.4 Verify Remote
```powershell
git remote -v
```

Should show:
```
origin  https://github.com/nahommesfin-ds/FinalProject.git (fetch)
origin  https://github.com/nahommesfin-ds/FinalProject.git (push)
```

---

## 📤 Step 3: Add & Commit Files

### 3.1 Check Status
```powershell
git status
```

### 3.2 Add All Files
```powershell
git add .
```

Or add specific files:
```powershell
git add FinalProject.ipynb
git add FINALPROJECT_README.md
git add requirements.txt
```

### 3.3 Create Commit
```powershell
git commit -m "Initial commit: FinalProject - Sleep Quality Analysis

- Comprehensive statistical analysis of 374 working professionals
- Investigates occupational stress, lifestyle factors, and sleep disorders
- Includes exploratory analysis, hypothesis testing, and predictive modeling
- Multiple statistical tests (ANOVA, Chi-Square, Mann-Whitney U)
- Logistic regression model with ROC/AUC analysis"
```

---

## 🔼 Step 4: Push to GitHub

### 4.1 Set Default Branch
```powershell
git branch -M main
```

### 4.2 Push to GitHub
```powershell
git push -u origin main
```

### 4.3 Enter Credentials (if prompted)
- **Username**: Your GitHub username
- **Password**: Your GitHub personal access token (see below if you don't have one)

---

## 🔐 Setting Up Personal Access Token (If Needed)

If Git asks for a password, use a **Personal Access Token** instead:

1. Go to [GitHub Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens)
2. Click **Generate new token (classic)**
3. Name: `git-cli`
4. Expiration: 90 days (or your preference)
5. Scopes: Check `repo` (Full control of private repositories)
6. Click **Generate token**
7. **Copy the token** (you won't see it again!)
8. Paste as password when Git prompts

---

## ✨ Step 5: Verify Your Work

1. Go to your GitHub repository: `https://github.com/nahommesfin-ds/FinalProject`
2. You should see:
   - ✓ FinalProject.ipynb
   - ✓ FINALPROJECT_README.md
   - ✓ requirements.txt
   - ✓ .gitignore
   - ✓ All files with your commit message

---

## 📝 Step 6: Rename README (Optional but Recommended)

In your GitHub repo:
1. Go to your repository
2. Click on `FINALPROJECT_README.md`
3. Click the three dots → **Rename**
4. Change to `README.md`
5. Click **Commit changes**

This way, GitHub will automatically display it on your repo home page!

---

## 🔄 Future Updates

After you make changes to your notebook, update GitHub:

```powershell
cd C:\pubh1142

# Check what changed
git status

# Add changes
git add .

# Commit with message
git commit -m "Updated analysis results and visualizations"

# Push to GitHub
git push origin main
```

---

## 🐛 Troubleshooting

### Error: "fatal: not a git repository"
- Make sure you ran `git init` in the correct directory
- Verify: `pwd` or `cd` to see current location

### Error: "fatal: 'origin' does not appear to be a 'git' repository"
- Run: `git remote add origin https://github.com/YOUR_USERNAME/FinalProject.git`

### Error: "Permission denied (publickey)"
- Set up SSH keys or use personal access token (see Step 5)

### Error: "Your branch is ahead of 'origin/main'"
- Run: `git push origin main`

### Want to see your commit history?
```powershell
git log --oneline
```

---

## 📱 Show Your Work!

After pushing, you can:

1. **Share the link**: `https://github.com/nahommesfin-ds/FinalProject`
2. **Add to your resume/portfolio**
3. **Share on LinkedIn** with a link to your analysis
4. **Tweet/Share**: "Just pushed my FinalProject - comprehensive analysis of sleep disorders using Python & data science 🛌 📊 #DataScience #PublicHealth"

---

## 🎯 What's Next?

After your project is live:

✅ Add a **Star** count badge to your README  
✅ Set up **GitHub Pages** to showcase the project  
✅ Create **Issues** for future improvements  
✅ Document how others can contribute  
✅ Keep the code updated as you learn more  

---

## 📚 Helpful Resources

- [GitHub Hello World](https://guides.github.com/activities/hello-world/)
- [Git Cheat Sheet](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
- [GitHub Docs](https://docs.github.com/en/get-started)

---

## 💬 Need Help?

If you run into issues:
1. Check your git status: `git status`
2. Check your remotes: `git remote -v`
3. Check your commits: `git log --oneline`
4. Google the error message + "github"

---

**You're all set! Your FinalProject is ready to share with the world! 🚀**
