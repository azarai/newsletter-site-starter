# LetterPage Newsletter Site Template


## Quick Start

### 1. Deploy via Netlify

[Deploy to Neltify](https://app.netlify.com/start/deploy?repository=https://github.com/azarai/newsletter-site-starter)

Click the button and follow the instructions. Netlify guides you through the setup. Customization is done via environment properties.

Unfortunately, Netlify does not keep order of those, so the pages might look a bit messy. Sorry, but that's out of my control.

### 2. Set up a Cron on Zapier, Integromat or alike

When deployed on Netlify the template defines the _UpdateArchive_ webhhok. You'll find that url under site settings - build and deploy - build hooks.

Create a Zap or similar that calls this URL with a POST request on your interval. Or call it manually, see command in your Netlify section.


## Manual Build & Deploy

The template uses Gridsome to build the site.

Build your site with `gridsome develop` and than deploy the dist directory to your hoster.

**Note** Auto-Update of the archive will not work with manual deploys. Best is to connect your Github repository to Netlify and use a build hook for the updates.

#### Install Gridsome CLI tool if you don't have

`npm install --global @gridsome/cli`

#### Customize Locally

Use `gridsome develop` to start a local dev server at `http://localhost:8080` and to debug your iste.