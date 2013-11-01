# Teleporter.io

The website for [Teleporter.io](http://teleporter.io).

## Overview

Our website is run over [Harp](https://github.com/sintaxi/harp), which is a simple static file server written in Node.js. 

## Installation

1. Checkout the repository: `git clone https://github.com/teleporter/teleporter.io.git`
2. Install Harp: `sudo npm install -g harp`
3. Run the harp server `harp server _site`

## Development

**Note:** *All development must be done in the `_site` folder.*

Running `harp server _site` will automatically compile assets on the fly.

When ready to deploy, run `harp compile _site ./` which will compile all the jade/sass/coffeescript/etc.. files into HTML/CSS/JS. 

Once compilation is finished, commit changes and push to Github. Github pages will automatically compile the site.

## Writing a post

Writing a post is a two part operation. First, create a new Markdown file in the `articles` directory (e.g. `kittens-wearing-hats.md`) and put in your content.

Then, modify the `articles/_data.json` file by adding in your article's title and publication date.

That's it! The application will automatically display your article in the articles `index.jade` template.
