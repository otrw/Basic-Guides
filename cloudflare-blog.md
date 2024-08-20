1. Prepare your Hugo site:
	- Ensure your Hugo site is ready and working locally.
	- Commit all your changes to your Git repository.
	- Push your Hugo project to a GitHub repository if you haven't already.

2. Sign in to Cloudflare:
	- Create a Cloudflare account if you don't have one.

3. Set up Cloudflare Pages:
	- Log in to your Cloudflare dashboard.
	- From the menu on left, click the Workers & Pages section.
	- Click the Pages tab and select Connect to Git and login to Git.

4. Configure your project:
	- Choose your GitHub repository.
	- Set your build settings:
		- Build command: `HUGO_ENV=production hugo --minify`
		- Build output directory: `public`
	- Click Save & Deploy
 
 Cloudflare will build and deploy your site and provide a URL.
 
5. Click Continue to Project

This will open the Workers & Pages / Blog (or whatever you called your site) section.

6. Click on the Custom domains tab
	- Click the Set up a custom domain button.
	- Enter in a registered domain or subdomain you own, click Continue.
	- Verify the DNS record is pointing to the correct pages.dev url set up earlier and then click Activate domain.

Note: This assumes the domain was purchased via Cloudflare. If the domain was purchased or is held elsewhere, update the relevant DNS records at your provider. Cloudflare will prompt you to do so in this step.

The domain setup and initialisation will start and will update with Active once completed.

Cloudflare will automatically deploy changes when you push to your GitHub repository.
