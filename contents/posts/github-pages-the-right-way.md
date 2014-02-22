---
title: "GitHub Pages: Custom Domains the Right Way"
date: 2014-03-01
template: post.jade
---

This is a quick guide for setting up custom domains with GitHub Pages. There is a common pitfall when naming your repo that can have far reaching consequences on other repos using GitHub Pages. I'll describe what to avoid and the best practices for doing it right.

If you ever want to use a custom domain, don't name your repo username.github.io. If you do this and you use a custom domain with it, all other repos under your account will inherit this domain for any Pages of their own. There's a small advantage to hosting project pages on github.io. You're demonstrating that you're open source, hosted on GitHub, right from the domain. There's a level of trust that comes with that. If you ever have contributors, they will be contributing to your *GitHub project,* not your personal site.

Instead, name your site *anything* else. One common convention is to use the domain name as the repo name. For my personal site, my repo is [willklein/willkle.in](https://github.com/willklein/willkle.in). Another idea is to just call it something simple, like blog, or personal-site.

You can even still use username.github.io as a root, and link to all your other project pages. Just don't use a custom domain there, that's really the only thing to avoid!