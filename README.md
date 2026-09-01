## 🚀 Deploying to Netlify via GitHub

This project is configured for continuous deployment to **Netlify** directly from this GitHub repository. Any changes pushed to the `main` branch will automatically trigger a new production build.

### Prerequisite
* A free or team [Netlify Account](https://netlify.com)

### Step-by-Step Connection Guide

1. **Log In to Netlify:**
   * Go to the Netlify dashboard and click **Log in**.
   * Select **GitHub** to authenticate your account.

2. **Add a New Site:**
   * Click the **Add new site** button on your team overview page.
   * Select **Import an existing project** from the dropdown menu.

3. **Authorize GitHub:**
   * Under *Connect to a Git provider*, click **GitHub**.
   * (Optional) Follow the prompts to authorize the Netlify GitHub App for either *All Repositories* or *Only Selected Repositories*.

4. **Select This Repository:**
   * Search for and select **`YOUR-REPOSITORY-NAME`** from your repository list.

5. **Configure Build Settings:**
   * **Production branch:** `main` (or your preferred default branch)
   * **Build command:** `npm run build` *(update this based on your framework)*
   * **Publish directory:** `dist` or `build` *(update this based on your framework)*

6. **Deploy:**
   * Click **Deploy [Your Site Name]**. 
   * Netlify will pull the code, build the application, and provide you with a live URL.

### 🔄 Automatic Updates
Once connected, every **Pull Request** will generate a unique *Deploy Preview* URL for testing. Merging a PR into your production branch will automatically update the live site within a few minutes.
