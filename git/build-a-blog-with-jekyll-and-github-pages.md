# Build a Blog with Jekyll and GitHub Pages

## Getting Started with Jekyll

```
gem install jekyll

jekyll new <my-jekyll-site>

jekyll serve // build jekyll site to directory _site

```

Configuration settings (configuration.yml)

permalink: pretty
permalink: /:title

## Building and Customizing the Blog

### YAML Front Matter

YAML Front Matter block
- is used by Jekyll for maintaining data for page and its context.
- always appear at top of the file
- is put between --- and ---
- any file with YAML Front Matter block will be processed by Jekyll as special file
- [main] scss file needs YAML Front Matter block to be threated as special file

### Liquid Templates

- A template language (introduced by shopify)
- Can access Front Matter data and output to Templates

{{ liquid handle }}

## Hosting with GitHub Pages

Create a new branch gh-pages (The branch name must be gh-pages)

### Steps to hosting with User Pages
- Initialize a local repository for our project
- Add the repository to GitHub using a specific naming convention
- Wait for GitHub Pages to build the site - usually no more than 10 minutes
