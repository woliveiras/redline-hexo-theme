# Redline Hexo Theme

A blog theme for Hexo.io

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

Is to use `Disqus`, `RSS feed`, `SitemapXML`, `Git Deploy` and others:

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
```
