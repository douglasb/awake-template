---
title: MPA Hybrid Chassis
subtitle: 2021 Granade sale buy
category:
  - For Sale
author: Douglas Brown
date: 2022-05-31
featureImage: /uploads/mpa-chassis-hero.jpg
---
## MPA Hybrid Stock

I was thinking about building a rifle for hunting, but I've decided to go another route. This is an awesome chassis and given it was part of the last years Granade Sale, the perfect fit for someone, just not me.  Never been used and Barrel/Action screws are included.

## Nuxt.js

[Nuxt.js](https://www.nuxtjs.org) has the ability to generate static sites that are served on the JAM Stack, building plain old html files... but those html files are super-powered with Vue.js. What this means, is that pages have content "hard coded" into the html files for top-rate SEO scores but after initial page load behave as a traditional SPA with smooth page transitions, minimal data served between requests, etc. This means Awake is fast both on both the first page visitors hit and even faster on subsequent pages.

## Purge CSS

Awake uses the [Bulma](https://bulma.io/) framework for a starting place for styles but certainly doesn't use every style the Bulma framework provides. [Purge CSS](https://www.purgecss.com/) minimizes the css sent to the browser by removing any unused styles at compile time. You can read more about how Awake uses Purge CSS in this [post](/light-css-footprint).

## Opti-Image + Responsive Loader

[Opti-Image](https://www.npmjs.com/package/opti-image) is a little vue component I wrote to be able to serve images in the most performant way possible. It supports webp's for browser's that support it (though not using the webp functionality for Awake, yet...), lazy loading out of the box, and easy srcset management. [Responsive Loader (the Nuxt Flavor)](https://www.npmjs.com/package/nuxt-responsive-loader) auto optimizes image quality for best performance in the browser and creates multiple sizes for different devices. Combine these 2 together and all image on Awake are basically guaranteed to fly. 

## Font Awesome 5

Awake comes with Font Awesome 5 support out of the box, so you have a wealth of free quality icons at your finger tips. However, if you're used to using Font Awesome in the more traditional manner without a build step you may be thinking: "What about all those icons I don't actually use? Aren't they just bloat?" Not so with Awake, with webpack we can bundle only the icons we're using. This does mean an extra step of registering a new icon when you want to use it, but that's as easy as adding it to an array in `config/modules.js` like so: 

```
 icons: ['faTimes', 'faSearch', 'faEnvelope', 'faUser', 'faBriefcase']
```

## Lazy Loading Like Crazy

In order to speed up both compile time and page load time, basically everything but the header, footer, hero, and main content of the posts are lazy loaded. All grids are lazy loaded with infinite scroll and all images (feature images and those in posts) are also lazy loaded. Comments can be lazy loaded or loaded on click of "Show Comments" button.

## Pretty Stinkin' Fast, I'd Say

I've taken a number of steps to try and make Awake as fast and snappy as possible for the end user and I think you'll find it's been handled fairly well. Last I ran one of the posts through Page Speed Insights I got a 99 score for desktop and 89 for mobile. [Give it a try for yourself!](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fawake-template.netlify.com%2Fpost-markup-and-formatting%2F&tab=desktop)

![Page speed insights score 99!!](/uploads/page-speed-insights.jpg)
