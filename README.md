# Storytelling Website

This is the website submodule repo for the [company's main website](http://trance-hd.github.io). We are using Hugo, a static site generator. This repo is the source files with a deploy script that can deploy its public assets to the website repo.

## Installation

Be sure to have Hugo installed.

### With Brew

```bash
brew update && brew install hugo
```

## File Organization

We're using the [dimension]() theme.
Any changes to the theme will be in the other folders.
For example, if we need to make changes to `theme/dimensions/layouts/index.html`,
we have to copy that file and add that to `layouts/index.html` and edit that file.
Same goes for assets.

## Deployment

Make sure `deploy.sh` is executable.

```bash
chmod +x deploy.sh
```

Deployments are automatic with the deploy script.
- This repo is a git submodule to the website repo
- The website repo holds all of the `public` assets for the static website

The following command will deploy the site changes straight to the public folder on the website repo.

```bash
./deploy.sh "Message for commit"
```
