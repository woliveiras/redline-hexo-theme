# Redline Hexo Theme

A blog theme for Hexo.io

## Demo

[Look here](http://woliveiras.com.br/redline-hexo-theme/).

## Install

After start your [Hexo Blog](https://hexo.io/docs/), open the blog folder on Terminal and run this:

```
git clone git@github.com:woliveiras/redline-hexo-theme.git themes/redline
```

Find the line:

```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: landscape
```

And change theme to `redline`.

Run `hexo serve` and look on `localhost:4000` if is all OK.

## Configuration

On file `themes/redline/_config.yml`, change this lines to your configs:

```
# Header
blog_title: Red Line
subtitle: Blog Theme

menu:
  home: /
rss: /atom.xml

# Content
excerpt_link: Continue reading...
fancybox: true

# Miscellaneous
google_analytics: UA-XXXXXXXX
favicon: img/favicon.png
twitter: your-twitter
facebook: your-facebook
linkedin: your-linkedin
github: your-github
```

## Extras

On `extra` folder have two files:

* _config.yml
* package.json

It's to use Disqus, RSS feed, SitemapXML, Git Deploy and others on yout Blog. Move to root (/) of Blog folder if you need more. ;)

**package.json**

```
{
  "name": "redline-blog-theme",
  "version": "0.0.0",
  "private": true,
  "hexo": {
    "version": "3.2.0"
  },
  "dependencies": {
    "hexo": "^3.2.0",
    "hexo-browsersync": "^0.1.1",
    "hexo-deployer-git": "0.0.4",
    "hexo-generator-archive": "^0.1.4",
    "hexo-generator-category": "^0.1.3",
    "hexo-generator-index": "^0.2.0",
    "hexo-generator-seo-friendly-sitemap": "0.0.15",
    "hexo-generator-tag": "^0.2.0",
    "hexo-renderer-ejs": "^0.2.0",
    "hexo-renderer-stylus": "^0.3.1",
    "hexo-renderer-marked": "^0.2.10",
    "hexo-server": "^0.2.0"
  }
}
```

**_config.yml**

```
# Hexo Configuration
## Docs: https://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/

# Site
title: Hexo
subtitle:
description:
author: Your name
language:
timezone:

# URL
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: http://yoursite.com
root: /
permalink: /:title/
permalink_defaults:

# Directory
source_dir: source
public_dir: public
tag_dir: tags
archive_dir: archives
category_dir: categories
code_dir: downloads/code
i18n_dir: :lang
skip_render:

# Writing
new_post_name: :title.md # File name of new posts
default_layout: post
titlecase: false # Transform title into titlecase
external_link: true # Open external links in new tab
filename_case: 0
render_drafts: false
post_asset_folder: false
relative_link: false
future: true
highlight:
  enable: true
  line_number: true
  auto_detect: false
  tab_replace:

# Category & Tag
default_category: uncategorized
category_map:
tag_map:

# Date / Time format
## Hexo uses Moment.js to parse and display date
## You can customize the date format as defined in
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss

# Pagination
## Set per_page to 0 to disable pagination
per_page: 10
pagination_dir: page

# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: redline

# Feed
feed:
  type: atom
  path: atom.xml
  limit: 20

# Disqus
disqus_shortname: your-disqus-shortname

# Deployment
## Docs: http://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: git@github.com:youruser/yourrepo.github.io.git
  branch: master

#SEO
sitemap:
    path: sitemap.xml
```
