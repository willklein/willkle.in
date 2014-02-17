---
title: Moving to Wintersmith
date: 2014-02-17
template: post.jade
---

I finally moved [willkle.in](https://github.com/willklein/willkle.in) to a proper static site generator: [Wintersmith](http://wintersmith.io). I've been testing Wintersmith for a while, and this past week I finally ironed out the details. I started with straight HTML, including some [Bootstrap](http://getbootstrap.com/), JS analytics, and [Disqus](http://disqus.com/). It took a while to port my HTML into [Jade](http://jade-lang.com/) templates and to get the content flowing correctly. There's more I plan to do, but here's my progress so far.

I decided to stick with [GitHub Pages](http://pages.github.com) for hosting, which includes [Jekyll](http://jekyllrb.com/) out of the box. Jekyll works fine and I used it for [HartfordJS.com](http://hartfordjs.com), but I wanted something more customizable. GitHub Pages restricts [custom plugins](http://jekyllrb.com/docs/plugins/) for security reasons, which is a bit limiting. I can still use GitHub Pages for free hosting, as long as I keep my build process offline or elsewhere.

Being a JavaScript/Node guy, Wintersmith was an excellent place to start. [Johan Nordberg](https://github.com/jnordberg) did a terrific job making it [extensible](https://github.com/jnordberg/wintersmith/wiki/Plugins), providing excellent support on GitHub and [Stack Overflow](http://stackoverflow.com/questions/tagged/wintersmith). Wintersmith is actually written in CoffeeScript, though that shouldn't matter much. I reviewed the source to figure out how things work and found the code very easy to follow. Johan made it relatively easy to extend by providing a [plugin template](https://github.com/jnordberg/wintersmith-plugin) and [API documentation](http://wintersmith.io/docs/). There are plenty of template engines supported; I stuck with Jade, the default. Jade has HAML-like syntax, which doesn't look anything like HTML at first glance. It can honestly be a pain to learn at first, but I've enjoyed the "shorthand" style of authoring HTML. Besides plugins, Wintersmith can also be customized by including other Node modules. I included [Lo-Dash](http://lodash.com) for util functions and [Moment.js](http://momentjs.com/) for date formatting. I could then use those libs directly in my Jade templates.

The last piece of the puzzle for me was auto-deployment. My desired workflow:

1. Create a new Markdown file.

2. Push that file to GitHub.

That's it. I wanted to edit a single file and have that publish without any fuss. I love how GitHub Pages works this way for Jekyll-based sites, and fortunately, I found a third-party service that helps fill this gap for Wintersmith. [Wercker](http://wercker.com) bills itself as an "open delivery platform." What it really does is it lets you write build scripts, hook into GitHub, and auto-build/deploy whenever you push to your repo. I found a very helpful [blog post](http://luke.vivier.ca/wintersmith-with-wercker/) explaining step-by-step how to wire up Wintersmith with GitHub Pages. Wercker also [wrote up](http://blog.wercker.com/2013/07/25/Using-wercker-to-publish-to-GitHub-pages.html) how to publish anything to Pages. I *really* like how Wercker can be used for a lot more than this, like continuous integration, or anything automated. It's free to try while in beta, so check it out.

This publishing workflow is very much a hacker's solution. I really enjoyed piecing it together, and it's highly extensible from here. Up next, I'm planning to rebuild my HTML & CSS on Bootstrap 3. I'm also hoping to build more on Wintersmith, more on that to come.