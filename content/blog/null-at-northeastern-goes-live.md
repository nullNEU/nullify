---
title: "null at Northeastern Goes Live!"
date: 2024-09-12T12:36:12-04:00
draft: false
readingTime: 3
---

This is it—the [official website](https://nullneu.pages.dev/) of null at Northeastern University is live 🥳

Let us delve into some behind-the-scenes details about what makes this amazing website work and why we are so proud about it.

## What's special...?

The website is built with [Hugo](https://gohugo.io/)—an open source static site generator framework written in Go. Leveraging the power of [markdown](https://en.wikipedia.org/wiki/Markdown) files for content management, html files for layouts, and CSS files for styling, we built a minimalistic website that helps communicate our ideas effectively.

Our website is blazingly fast—deploying it on [Cloudfare Pages](https://pages.cloudflare.com/) gave us the added benefit of [DoS protection](https://www.cloudflare.com/learning/ddos/what-is-a-ddos-attack/), caching and high availability via the global Cloudfare CDN, and SSL certificates out-of-the-box.

Keeping in mind the diverse usage patterns of our members and well-wishers, we have built the website to work on any browser and device. At null, we are all for inclusiveness!

If this gets you intrigued to know more about how we built our website, we have you covered. The [codebase for this website](https://github.com/nullNEU/nullify) is fully open-source—so you can peruse, inspect and report any inaccuracies you may find in the codebase, or make a contribution yourself.

### Secure from the ground up

When we say secure, we mean secure in all aspects—runtime to deployment.

Apart from generating static HTML files at incredible speeds, Hugo is inherently more secure than other SSG frameworks like WordPress which rely on an external database for site generation. Each component of this website including styling files, media files and content files are scanned for vulnerabilities by [Hugo's internal security policies](https://gohugo.io/about/security/) before being mounted onto the site's file system. This reduction in attack vectors cuts down the possibility of exploits being carried out on the site while still in development or otherwise.

Additionally, since Hugo is built on top of Golang, [performance efficiencies offered by the language](https://www.golinuxcloud.com/golang-performance/) also apply to websites built with Hugo. Aside from requiring very little boilerplate code to get the site up and running, Golang internally provides one of the fastest and secure back ends for the website to run on.

We went one step further. At the time of writing this blog, we ship zero JavaScript—there are no client side scripts that are executed on the browser. Apart from improving the speed of the website considerably—and making code easier to maintain without managing numerous npm packages—this also means that there is no cross session tracking or attempting to get any of your valuable data.

## Some stats

The website went live on 2nd September, 2024. At the time of writing, we have received 380 hits, with almost 92% being from mobile devices. We know what media queries to target now :)

We ran our website through [PageSpeed Insights](https://pagespeed.web.dev/) (PSI), a service provided by Google that measures web performance. Scoring a 100% for our desktop version and 93% for the mobile version, we have a page load time of just 620 ms. With high scores for accessibility and SEO, our website ticks most boxes!

## What's next?

We think the website is great, but it can be better. To make it the best, we need your support, opinions, and contributions. You can [star the repo on GitHub](https://github.com/nullNEU/nullify) to let us know you loved it, raise a [new issue](https://github.com/nullNEU/nullify/issues) on GitHub to give us suggestions or tell us about bugs we might have missed, or [raise a new PR](https://github.com/nullNEU/nullify/pulls) with your code changes!

We're waiting to see your name on our contributors' list!

 

