# Welcome to Ram Robotics

This website is built using the github page theme "minimal". The HTML and CSS are generated with jekyll, so new pages are writen in markdown and later parsed to HTML.

## How build the website locally:

Follow steps to build the site locally: [instructions](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll?platform=windows#building-your-site-locally)

In summary:
1. ensure you have ruby installed with `ruby -v` 
1. install bundler with `gem install bundler`
1. run `bundle exec jekyll serve --baseurl=""` to serve website locally

## How to publish new version of website.

Make sure you have tested your changes to the website in your `feature-branch`. Create a Pull Request to the branch `publish`, have it reviwed and merged to `publish`. The website will be automatically updated. Make sure this was actually set up following the instructions here: [Publishing from a branch](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-from-a-branch)


## How to create pages:

Website pages correspond to `.md` files in the root folder of the project. The `index.md` page is special because it will be shown when a user opens [https://ramroboticsunc.github.io/](https://ramroboticsunc.github.io/). Any new `.md` files that follow the website header

```
---
layout: default
---

# Page Title
```
will render as new pages in the url [https://ramroboticsunc.github.io/new-page.html](https://ramroboticsunc.github.io/new-page.html)

To link to a page called `new-page.md`, add a link in this format to the markdown of the page:
```
[Link to another page](./new-page.html).
```

More instructions on [Adding a new page](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll#adding-a-new-page-to-your-site)


## How to add images:

Upload your file to `assets/img`. Use the new image in your page with the following:
```
![Alt text for your image](/assets/img/your-image.jpg)

```

## New Github Page from a theme

If you want to start from scratch and build the website from a new theme, follow these instructions [Create new site from scratch](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site)

## Consider the limitations of github pages

Read the [usage limits](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits) on github pages.