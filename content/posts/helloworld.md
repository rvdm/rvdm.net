---
title: "Hello, world"
date: 2024-10-13T18:55:41+02:00
draft: false
---

So, I guess this is another attempt at a website. I need one a bit more now, due to wanting to share some information on my [peering](https://rvdm.net/bgp/) setup.

For the site, I'm using the static site generator [hugo](https://gohugo.io) along with some tricks with Github Actions, Github Pages, and a reverse proxy to host everything on my own domain name without having to pay for things.

Should you want to set up a similar thing, the repositories are open. 

The source of this site can be found on github [here](https://github.com/rvdm/rvdm.net). I use this repository to keep config, theme and markdown content. 
Once I push to the repo, a github action is started that renders the static content, and pushes it to another [repository](https://github.com/rvdm/rvdm.github.io). 

The second repository is github pages-enabled and serves the content. 
Finally, I'm using nginx' proxy_pass config to reverse-proxy the content (and to serve it on the actual domain name). That config is not published anywhere, but easy enough to do.
