# Deploying to Vercel

## Option 1: Using Vercel CLI (Recommended)

1. **Install Vercel CLI** (if not already installed):

   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**:

   ```bash
   vercel login
   ```

3. **Deploy**:

   ```bash
   vercel
   ```

   - First time: Follow prompts to link to a Vercel project
   - Production: Use `vercel --prod` for production deployment

## Option 2: Using Vercel Dashboard

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "Add New Project"
3. Import your Git repository (GitHub/GitLab/Bitbucket)
   - OR drag and drop your project folder directly
4. Configure settings (usually auto-detected for static sites)
5. Click "Deploy"

## Option 3: Using GitHub Integration

1. Push your code to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → Dashboard
3. Click "Add New Project" → Import Git Repository
4. Select your repository
5. Vercel will auto-detect settings and deploy

## Accessing Your Deployed Site

After deployment:

- **Development**: `https://your-project-name.vercel.app`
- **Production**: Your custom domain or the provided `.vercel.app` URL

## Testing Your Player

Once deployed, test your player with:

```
https://your-project-name.vercel.app/player.html?vid=VIDEO_ID
```

Example:

```
https://your-project-name.vercel.app/player.html?vid=jNQXAC9IVRw&autoplay=1&mute=1
```

## Your Current Configuration

Your `vercel.json` is already configured with:

- Clean URLs enabled
- No trailing slashes

This is perfect for your static HTML files!
