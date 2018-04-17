# Gatsby Blog Starter

First part of the tutorial series on creating a blog with [GatsbyJS](http://gatsbyjs.org) on [Stay Regular](http://stayregular.net/blog).

## Install

Clone from repo:
```sh
git clone https://github.com/whoisryosuke/gatsby-blog-tutorial.git gatsby-example-site
```

Make sure that you have the Gatsby CLI program installed:
```sh
npm install --global gatsby-cli
```

Then you can run it by:
```sh
cd gatsby-example-site
npm run develop
```

## Deploy

### Github Pages

1. Create a git repo inside your project.
2. Add your Github hosted repository as a remote repository named origin:
```sh
git remote add origin http://github.com/username/repo-name.git
```
3. Change the pathPrefix in `gatsby-config.js` to your Github repository's name.
4. Commit any changes with git to the master branch. Then run:
```sh
npm run deploy
```

### Netlify

1. Click the following button, connect your Github account, and create a new repo.
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/whoisryosuke/gatsby-blog-tutorial)
2. Go to the Deploys section, then click the Deploy settings button.
3. Under Continuous Deployment, the first box should be Deploy Settings. Click Edit Settings at the bottom of the container.
4. Change your Build command to `npm run build`
5. Change your Publish directory to `public`
6. Make sure the branch is master, or your preferred production branch.
![Settings on Netlify](https://i.imgur.com/WcaXqOx.png)
7. Click Save.
8. Go to the Deploys section again and click Trigger deploy. Make sure the clear cache is checked, and run the deploy.
