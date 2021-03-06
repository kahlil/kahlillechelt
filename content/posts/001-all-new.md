---
title: "All New"
date: 2017-09-15
---

My blog used to be a Medium publication with a linked domain but I ditched Medium. I was disappointed with the design directions they are taking.
I was a big fan of Medium's design before the recent change to the new serif wordmark. It feels disjointed to me now and it is apparent that they are pushing their paid services and are working hard to make an _actual_ business out of Medium. That's all good and fine but I don't like the changes and that made me realize I need to have more control over my blog again.

Also I wanted to consolidate kahlil.info and kahlillechelt.com. So here we are. New blog same old me.

For now I am leaving my old blog posts [over there on Medium](https://medium.com/@kahlil). I will port them over eventually. Maybe. I will be cross posting my blog posts from here over at Medium as well. The readership you get over there via their network is really nice.

## Design

The initial inspiration for the design was a quick study that [@magalhini](https://twitter.com/magalhini) posted to Twitter a while ago. I played around with it but wanted a different font pairing. After some googling I found [Typewolf Google Fonts](https://www.typewolf.com/google-fonts) and [Great Simple](http://fonts.greatsimple.io/rubik-roboto/), two websites that suggest Google font pairings. I ended up choosing [Roboto Mono](https://fonts.google.com/specimen/Roboto+Mono) as a main font and [Rubik](https://fonts.google.com/specimen/Rubik) for my wordmark.

I found the pairing [here](http://fonts.greatsimple.io/rubik-roboto/) and after I saw it I kept coming back to it. So I went with it. I really like using a monospace font for the body text.

I am happy with it. Keeping it simple.

## It's A Static Site

As a web developer I _have_ to use a static site generator of course. Which one you ask?

[Hugo](http://gohugo.io)!

Hugo is written in Go and comes as a binary. It's wicked fast and can easily deal with huge amounts of posts.

It has been around for a while now and is really flexible. It works very similarly to other static site generators like Jekyll or Metalsmith.

## Hosting

For hosting I went with [Netlify](http://netlify.com), I've been really impressed with their user experience for hosting static pages. If your site is on Github it is incredibly easy to  deploy it to Netlify:

- link your Github respository
- tell them the command that builds your site
- tell them the name of the folder that the built site end up in

Done!

The site gets redeployed every time you push to master (this feature can be turned off) and if I push a branch to the site's Github repo Netlify will attempt to deploy a preview automatically. It's truly a joy to use.

If you are interested in the code for this site you can find it [on Github](https://github.com/kahlil/kahlillechelt.com).
