# Individual KPI Dashboard

Deploy this interactive dashboard to various hosting platforms:

## 🌐 Deployment Options

### 1. Netlify (Recommended - Free)
- Drag and drop the entire folder to [Netlify Drop](https://app.netlify.com/drop)
- Or connect your GitHub repo at [Netlify](https://netlify.com)

### 2. Vercel (Free)
- Import your GitHub repo at [Vercel](https://vercel.com/import)
- Zero configuration needed

### 3. GitHub Pages (If repo is public)
- Go to repo Settings > Pages
- Select "Deploy from a branch" > main > / (root)

### 4. Firebase Hosting (Free)
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

### 5. Surge.sh (Free)
```bash
npm install -g surge
surge
```

## 📁 Files to Deploy
- `NblyIndividualTracker.html` (main dashboard)
- `index.html` (redirect page)
- `README.md` (documentation)
- `netlify.toml` (Netlify configuration)

## 🔗 Public URLs
Once deployed, your dashboard will be accessible at:
- **Netlify**: `https://your-site-name.netlify.app`
- **Vercel**: `https://your-repo-name.vercel.app`
- **GitHub Pages**: `https://username.github.io/repo-name`