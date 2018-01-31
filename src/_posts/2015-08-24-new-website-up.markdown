---
layout: post
title: The new website is finally up
date: '2015-08-24 19:00:00'
---

Hello, fellow readers. In this post I want to introduce you to the new website,
including some technical details for reference.

## The old website

<img class="cld-responsive" data-src="//res.cloudinary.com/mattiascibien/image/upload/c_scale,h_800,w_1280/v1440408038/old-website_ashu9y.png"/>

The old website was actually a static single page developed with the [Bootstrap](getbootstrap.com/)
framework alongside a blog residing into the blog subdomain made with [Ghost](https://ghost.org/).

While Ghost is a wonderful blogging platform and I have even did some work on 
the engine, at the moment, it is difficult to update from one version to the next
one; every time I wanted to write a post, which was a rare event, 
I always found out that I needed to do a Ghost update, which is somehow time 
consuming. 
Obviously, after all the update I did not want to write the post anymore 
(I still have other things to do, a wife and a life away from the keyboard).

Moreover, both website and blog did not share the same theme. I tried to make
the same theme for both the website and the blog but due to the nature of the 
static site and the blog I had to duplicate a lot of files. The result can be
seen on the [ghostmatt theme repository](https://github.com/mattiascibien/ghostmatt/).
Ghostmatt is actually now available (unfinished) under the MIT license and therefore can be
used in your Ghost blogs. It has even some nice jQuery plugins like my custom 
version coinbox for cryptocurrency donations.

## Root, the revolution

The new website is actually the 20th (or even more, I lost the count) iteration
of my web space and I guess it is something I will keep for a while since I
finally managed to have a website that is fully customizable, easy to maintain
and easy to blog with.

It's codename is Root, which has been chosen actually because it is going to be 
the very top in the hierarchy of my websites (the sub ones about [AnimaRender](http://mattiascibien.github.io/Anima-Render) and
[IvyGen](http://mattiascibien.github.io/ivygen) are going to be moved under the github.io domain, which is actually where
they belong) and also because it is really *Kick-Ass Awesome*, much like the
character form the series [Person Of Interest](http://personofinterest.wikia.com/wiki/Root).
These where actually my inspirations for the name.

### Jekyll, static blogs and websites

As you can see the whole website is now a bunch of static files which are served
form my Rack server with no database nor server processing. This decision has
actually been made to provide the visitor the maximum achievable performance and
response time.

Thanks to Jekyll, a static website generator maintaining a website of this kind id
really simple. Every time I want to write a new post or change a page I just 
need to fiddle with some [markdown](http://daringfireball.net/projects/markdown/) f
iles which are then automatically processed by Jekyll applying layouts 
and common page elements, all done with minimun site downtime.

### The theme

The theme is actually a customized bootstrap theme made from a palette inspired 
by the Tron Legacy movie colors. Unfortunately I cannot find that palette anymore.

Thanks to [SASS](http://sass-lang.com/) I am now able to control every bit of the 
theme with just a bunch of variables.

### The new art gallery

The art gallery has always been broken on the old site. I actually host
all of my art on deviantART and there are no gallery solution providing tight 
integration with that so I had to develop a custom way to provide a nice image 
gallery experience here on my website, while keeping the images only in one place.

The new gallery simply reads my gallery MediaRSS from deviantART to provide
a nice grid with a lightbox made with the wonderfult [Magnific Popup](http://dimsemenov.com/plugins/magnific-popup/). To read the
RSS and parse it I used the great [deviantART-API](https://github.com/jamesl1001/deviantART-API) 
by [James Alexander Lee](http://jalproductions.co.uk/).

The whole gallery is anyway going to be expanded in the near future with the 
possibility to buy additional image-related content, share images on social networks and downloading
which needs to be done only on deviantART at the moment.

Due to the nature of some images I also added a simple disclaimer to prevent the
user eyes from imags which can be seen as offending (even if they are not in my
opinion).

### Contact me

In the end, I set up a simple contact form [here](/contact/) which can be used 
to write to me to ask about almost anything. I will try to respons as soon as possible.

## Conclusions

Well, this is actually how I made the beast called Root which empowers my website.
As any other piece of software, anyway, it is far from definitive, may contain
bugs and maybe it does not fit some tastes. I am always open to suggestions and
improvements so I have set up a [issue tracker on GitHub](https://github.com/mattiascibien/website)
where you can give help on fine-tuning the website.

Enjoy yor stay here at the new Mattias Cibien Website.

Mattias