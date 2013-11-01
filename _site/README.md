# Teleporter.io

The website for [Teleporter.io](http://teleporter.io).

## Overview

Our website is run over [Harp](https://github.com/sintaxi/harp), which is a simple static file server written in Node.js. 

## Installation

1. Checkout the repository: `git clone https://github.com/teleporter/teleporter.io.git`
2. Install Harp: `sudo npm install -g harp`
3. Run the harp server `harp server .`

## Development

Save changes to the templates and stylesheets and the Harp server will reload changes.

When ready to deploy, run `harp compile _site ./` and commit changes. Github pages will automatically compile the site.

## Writing a post

Writing a post is a two part operation. First, create a new Markdown file in the `articles` directory (e.g. `kittens-wearing-hats.md`) and put in your content.

Then, modify the `articles/_data.json` file by adding in your article's title and publication date.

That's it! The application will automatically display your article in the articles `index.jade` template.
