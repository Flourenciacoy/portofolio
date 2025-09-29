# Vercel Deployment Guide

## Prerequisites
- GitHub account
- Vercel account (sign up at vercel.com using your GitHub account)

## Step-by-Step Deployment Instructions

### 1. Prepare Your Repository
1. Create a new repository on GitHub
2. Push your portfolio code to the repository

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit your changes
git commit -m "Initial portfolio website commit"

# Add your GitHub repository as origin
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push to GitHub
git push -u origin main
```

### 2. Deploy with Vercel Website
1. Go to [vercel.com](https://vercel.com)
2. Sign in with your GitHub account
3. Click "New Project"
4. Import your GitHub repository
5. Configure the project settings:
   - **Framework Preset**: Other
   - **Root Directory**: ./ (default)
   - **Build Command**: Leave empty (static site)
   - **Output Directory**: Leave empty (static site)
   - **Install Command**: npm install

### 3. Environment Variables (if needed)
If you need to add any environment variables for your contact form:
1. Go to your project settings in Vercel
2. Navigate to "Environment Variables"
3. Add any required variables

### 4. Custom Domain (Optional)
1. Go to your project settings
2. Navigate to "Domains"
3. Add your custom domain
4. Follow Vercel's DNS configuration instructions

## Project Structure
```
portfolio/
├── index.html          # Main portfolio page
├── css/
│   └── style.css      # Styling with glass morphism effects
├── js/
│   └── script.js      # Contact form functionality
├── files/
│   ├── CV.html        # Resume page
│   └── profile.jpg    # Profile image
├── package.json       # Project metadata
├── vercel.json        # Vercel configuration
└── README.md          # Project documentation
```

## Key Features
- ✅ Modern responsive design
- ✅ Glass morphism effects
- ✅ Contact form with Google Sheets integration
- ✅ Experience and Education sections
- ✅ Performance optimized
- ✅ Fixed navigation bar

## Contact Form Integration
Your contact form is integrated with Google Apps Script at:
`https://script.google.com/macros/s/AKfycbxHYKtGSLIerRwVcGhCQwPd6aHoZdwOGpYIuCElqDPXRWOwxgvg7yweku6rjvmufA/exec`

Make sure this Google Apps Script is properly configured to receive form submissions.

## Troubleshooting
- If the site doesn't load properly, check the Vercel build logs
- Ensure all file paths are correct and case-sensitive
- Verify that your Google Apps Script URL is accessible and configured correctly

## Post-Deployment Checklist
- [ ] Test contact form functionality
- [ ] Verify all images load correctly
- [ ] Check responsive design on different devices
- [ ] Test navigation and smooth scrolling
- [ ] Verify Google Sheets integration works