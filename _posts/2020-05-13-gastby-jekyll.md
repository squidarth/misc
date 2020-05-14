---
layout: post
title:  "How I Built This"
date:   2020-05-13 10:18:00
categories: personal
---

_Obligatory musings about the state of blogging technology_

When deciding to make a new site, I had to face the eternal question of
"Do I reach for something I know how to use and does the job well or try
the new hotness?".

The new hotness, in this case, is [GatsbyJS](https://www.gatsbyjs.org/).

Gatsby has some pretty interesting ideas, and to be honest, took me a while
to understand. The main gist of it is that you write a React.js application,
and the Gatsby tool will take that, and at compile-time, run that application,
and spit out a static site.

This is cool, because the React.js application that you define could pull data
from a variety of data sources, but you *incur the cost* of pulling data from those
sources at compile-time, rather than when users are using the application. These
data sources could be literally anything, CMS data, markdown files, some external API.

All that said, for what I'm trying to accomplish with this site, this doesn't really buy
me anything. With either trusty old [Jekyll](https://jekyllrb.com/), which I used for squidarth.com,
or Gatsby, I'd be writing my posts in markdown files. I don't have any other data sources I
care about. It's possible that using React templating is nicer than the Jekyll templating,
but frankly, I don't plan on editing the templates very often (I will hopefully spend most
of my time in this project writing posts!).

So all that to say, I decided to opt for Jekyll this time around, with the [Kasper](https://jekyllthemes.io/theme/kasper)
theme.

Ugh, now I feel old.

##### Why not a CMS?

The thing that I definitely miss by writing posts in Markdown and using
these static-site generators is the ability to get edits. The options are basically--
write your post in a Google doc, get edits, and then copy it into Markdown, or make Github
pull requests and have people comment. The latter option just isn't the right tool for the job,
and the former is clunky.

I know some CMS tools support this better. However, I want the flexibility to embed code in these posts and
more do what I want, which is harder to do with CMSs.
