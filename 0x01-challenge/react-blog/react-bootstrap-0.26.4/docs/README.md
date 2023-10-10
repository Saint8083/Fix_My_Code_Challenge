React-Bootstrap Documentation Website
This website is single page app built on React, with styles and structure taken from the Bootstrap docs website. The app is statically generated to HTML via node and then hosted it by pushing HTML to GitHub Pages.

Development
From the repository root run npm run docs and navigate your browser to http://localhost:4000. This will start an express base node server with webpack-dev middleware that will watch your file changes and recompile all the static assets needed to generate the site. In the console output you'll see that we bind to two ports. The first port is the one you'll use to load the docs in your browser. The second is the webpack-dev-server we use to build the client side assets in watch mode. Note: while the docs should start on port 4000 if that port is in use we progressively look for an available port. Observe console output for the actual port that we use. We use the webpack and react hot loading functionality to allow your development experience to have quickest feedback loop possible.

For a demo of how the hot loader works checkout this video:

Demo of hot loader

Production
This site is statically published on github pages, to do this the static assets need to be generated. You can simulate a similar experience with npm run docs-prod and navigating your browser to http://localhost:4000
