# 🚀 Deployment Guide - CloudEagle Integration Builder

## Step-by-Step Deployment to Streamlit Cloud

### ✅ Prerequisites
- [x] You have an Anthropic API key
- [ ] You have a GitHub account (create one at github.com if needed)
- [ ] You have the code files ready

---

## 📤 Step 1: Push Code to GitHub

### Option A: Using GitHub Web Interface (Easiest - No Command Line)

1. **Go to GitHub.com and sign in**

2. **Create a new repository:**
   - Click the "+" icon in top right → "New repository"
   - Repository name: `cloudeagle-integration-builder`
   - Description: "AI-powered integration code generator for CloudEagle"
   - Set to: **Public**
   - ✅ Check "Add a README file"
   - Click "Create repository"

3. **Upload files:**
   - Click "Add file" → "Upload files"
   - Drag and drop ALL these files:
     - `app.py`
     - `requirements.txt`
     - `.gitignore`
     - `README.md`
   
4. **Upload .streamlit folder:**
   - Click "Add file" → "Create new file"
   - Name it: `.streamlit/config.toml`
   - Copy-paste the content from your local `.streamlit/config.toml`
   - Click "Commit changes"

5. **Done!** Your code is on GitHub

---

### Option B: Using Git Command Line (If you prefer)

```bash
# Navigate to your project folder
cd /path/to/cloudeagle-integration-builder

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: CloudEagle Integration Builder"

# Create main branch
git branch -M main

# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/cloudeagle-integration-builder.git

# Push to GitHub
git push -u origin main
```

---

## 🌐 Step 2: Deploy to Streamlit Cloud

1. **Go to Streamlit Cloud:**
   - Visit: https://share.streamlit.io
   - Click "Sign in"
   - Sign in with your GitHub account

2. **Create new app:**
   - Click "New app" button
   - Or click your profile → "New app"

3. **Configure deployment:**
   - **Repository:** Select `YOUR_USERNAME/cloudeagle-integration-builder`
   - **Branch:** `main`
   - **Main file path:** `app.py`
   
4. **Click "Deploy!"**

5. **Wait for deployment** (takes 2-3 minutes)
   - You'll see build logs
   - Status will show "Your app is live!" when ready

---

## 🔐 Step 3: Add Your API Key (IMPORTANT!)

After deployment starts:

1. **While app is deploying, click "Advanced settings"**
   
2. **Or after deployment, go to app settings:**
   - Click the ⋮ menu on your app
   - Select "Settings"

3. **Go to "Secrets" tab**

4. **Add your Anthropic API key:**
   ```toml
   ANTHROPIC_API_KEY = "sk-ant-api03-..."
   ```
   
   Replace with your actual API key from console.anthropic.com

5. **Click "Save"**

6. **App will automatically restart** with the new secret

---

## ✅ Step 4: Test Your App

1. **Get your app URL:**
   - Format: `https://YOUR_APP_NAME-RANDOM_ID.streamlit.app`
   - Example: `https://cloudeagle-integration-builder-abc123.streamlit.app`

2. **Visit the URL**

3. **Test the app:**
   - Click "Calendly" button
   - Click "Generate Integration Code"
   - Verify code generates successfully
   - Test download ZIP

4. **If there are errors:**
   - Check the app logs (click "Manage app" → "Logs")
   - Verify API key is correct in Secrets
   - Check that all files uploaded correctly

---

## 🎥 Step 5: Share Your App

Your app is now live! You can share it in your CloudEagle submission:

```
🚀 Live Demo: https://your-app-name.streamlit.app

Try it yourself:
1. Visit the link above
2. Click "Calendly" example
3. Click "Generate Integration Code"
4. Review generated code
5. Download ZIP file
```

---

## 🔧 Troubleshooting

### App won't start
- **Check:** Did you add `ANTHROPIC_API_KEY` in Secrets?
- **Check:** Is your API key valid? (test at console.anthropic.com)
- **Check:** Are all files uploaded to GitHub?

### Code generation fails
- **Check:** App logs for error messages
- **Check:** API key format (should start with `sk-ant-api03-`)
- **Check:** You have credits in your Anthropic account

### Files missing on GitHub
- **Solution:** Upload them via "Add file" → "Upload files"
- **Don't forget:** `.streamlit/config.toml` folder structure

### App URL changed
- **Normal:** Streamlit gives you a random URL on first deploy
- **Can't change:** The URL is fixed (unless you delete and redeploy)

---

## 🎯 What to Submit to CloudEagle

### Your Google Doc should include:

**Section: Working Prototype**

```markdown
## Prototype - Live Demo

I built a fully functional working prototype using Streamlit and Claude 3.5 Sonnet.

🚀 **Live Demo:** https://your-app-name.streamlit.app

### How to Test:
1. Visit the URL above
2. Click "Calendly" from popular integrations
3. Click "Generate Integration Code"
4. Review the 5 generated Python files
5. Download complete package as ZIP
6. Optional: Test sandbox mode

### Features Demonstrated:
- ✅ AI-powered code generation using Claude 3.5 Sonnet
- ✅ Beautiful, professional UI
- ✅ Automated safety checks
- ✅ Syntax-highlighted code preview
- ✅ Downloadable ZIP package
- ✅ Sandbox testing simulation

### Technical Implementation:
- **AI Model:** Claude 3.5 Sonnet (claude-sonnet-4-20250514)
- **Framework:** Streamlit (Python)
- **Deployment:** Streamlit Cloud
- **Code:** Available at github.com/YOUR_USERNAME/cloudeagle-integration-builder
```

---

## 📝 Quick Reference

**Your GitHub Repo:** `github.com/YOUR_USERNAME/cloudeagle-integration-builder`
**Your Live App:** `https://YOUR_APP_NAME.streamlit.app`
**Streamlit Dashboard:** `share.streamlit.io`

---

## 🆘 Need Help?

1. **Check app logs:** Streamlit Cloud → Your app → Logs tab
2. **Restart app:** Streamlit Cloud → Your app → Reboot
3. **Re-deploy:** Delete app and create new one with same settings

---

**Good luck with your submission!** 🚀
