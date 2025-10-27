# GitHub Profile Setup Guide 🚀

This guide will help you set up your enhanced GitHub profile with the snake game animation.

## 📋 Prerequisites

1. A GitHub account (username: `matulwan`)
2. A special repository named `matulwan` (same as your username)

## 🔧 Setup Steps

### Step 1: Create the Profile Repository

If you haven't already:
1. Go to GitHub and create a new repository
2. Name it exactly: `matulwan` (same as your GitHub username)
3. Make it **public**
4. Initialize with a README (or push this one)

### Step 2: Push Your Files

```bash
# Initialize git if not already done
git init

# Add all files
git add .

# Commit your changes
git commit -m "✨ Enhanced GitHub profile with snake game"

# Add your GitHub repository as remote
git remote add origin https://github.com/matulwan/matulwan.git

# Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Actions

1. Go to your repository on GitHub: `https://github.com/matulwan/matulwan`
2. Click on the **"Actions"** tab
3. If prompted, click **"I understand my workflows, go ahead and enable them"**
4. The snake animation workflow will run automatically

### Step 4: Manually Trigger the Workflow (Optional)

1. Go to **Actions** tab
2. Click on **"Generate Snake Animation"** workflow
3. Click **"Run workflow"** button
4. Select the `main` branch
5. Click **"Run workflow"**

The workflow will:
- Generate the snake animation from your contribution graph
- Create both light and dark theme versions
- Save them to the `output` branch
- Update automatically every 24 hours

### Step 5: Customize Your Profile

Edit the `README.md` file to personalize:

1. **About Me Section** (lines 28-34)
   - Update your bio, interests, and contact info

2. **Tech Stack** (lines 42-60)
   - Add/remove technologies you use
   - Find more badges at: https://shields.io/

3. **Social Links** (lines 94-97)
   - Replace placeholder links with your actual profiles:
     - LinkedIn: `https://linkedin.com/in/your-profile`
     - Twitter: `https://twitter.com/your-handle`
     - Portfolio: `https://your-portfolio.com`
     - Email: `your-email@example.com`

## 🎨 Features Included

### ✅ Animated Typing Header
Dynamic greeting with typing animation

### ✅ Profile View Counter
Tracks how many people visit your profile

### ✅ Tech Stack Badges
Visual representation of your skills with colorful badges

### ✅ GitHub Statistics
- Overall GitHub stats
- Most used languages
- Contribution streak

### ✅ Snake Game Animation
The snake eats your GitHub contributions! 🐍

### ✅ Random Dev Quote
Inspirational quote that changes on each visit

### ✅ Social Links
Quick access to your social profiles

## 🐛 Troubleshooting

### Snake Animation Not Showing?

1. **Wait for the workflow to complete**
   - Check the Actions tab for workflow status
   - First run may take 2-3 minutes

2. **Check the output branch exists**
   - Go to your repository
   - Click on the branch dropdown
   - Look for `output` branch

3. **Verify workflow permissions**
   - Go to Settings → Actions → General
   - Under "Workflow permissions", select "Read and write permissions"
   - Click Save

### Stats Not Loading?

- GitHub stats services may have rate limits
- Try refreshing after a few minutes
- Stats update automatically

## 🎯 Next Steps

1. ⭐ Star some repositories to show activity
2. 🔥 Make regular commits to build your streak
3. 🤝 Contribute to open source projects
4. 📝 Keep your profile updated with new skills

## 📚 Resources

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Shields.io - Badge Generator](https://shields.io/)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Snake Animation Action](https://github.com/Platane/snk)

## 💡 Tips

- Keep your README concise and scannable
- Update your profile regularly
- Showcase your best projects
- Use emojis sparingly for visual interest
- Make sure all links work

---

**Happy Coding! 🚀**
