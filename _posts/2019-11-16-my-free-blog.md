---
title: 'How I created a free blog.'
date: 2019-11-16 00:00:00
featured_image: '/images/2019-11-16/blog-screen.jpg'
excerpt: Expanding on my personal brand brought the need for me to create a blog. I wanted to share updates to my followers. I required a solution that did not have a monthly cost associated with it. I did not want to be hosted on a free tier solution that provided a subdomain like areyesjr.somecompany.com. I wanted areyesjr.com and I wanted it to look premium.
---

![](/images/2019-11-16/vscode.jpg)

## I found Jekyll!

I set a goal for myself during 2019 and that goal was to become extremely fluent in markdown. I started to research ways that I can practice and found jekyll. Jekyll is a parsing engine bundled as a ruby gem used to build static websites and is perfect to practice markdown!.
 
> "Local development is a requirement! "

I always strive to do things different and I did not want to build another wordpress site. I wanted a solution that would allow me to develop locally (offline) in my mac then push to github once I was ready for production. The combination of [Cloudflares](https://www.cloudflare.com/) free cdn and [Github Pages](https://pages.github.com/) pages provides a very strong combination with no monthly cost. 

### Free and Premium themes.

I am currently using a premium theme and I hope to keep it as a secrets but you can always access the code in my Github profile and figure it out. For free versions there are a bunch out there just Google free Jekyll themes. 

Here are a couple of free themes:

* [https://jekyllthemes.io/free](https://jekyllthemes.io/free)
* [http://jekyllthemes.org/](http://jekyllthemes.org/)
* [https://jekyllrb.com/resources/](https://jekyllrb.com/resources/)

### How is the installation?

Well, its pretty simple just edit the themes once you have configured them and push them out to your github. 
For custom domains you would want to make sure you are pointing DNS to github pages. You can find instruction on Github Pages [here](https://guides.github.com/features/pages/). 

Once you have your theme modified to your liking you just need to create an account with [Cloudflare](https://www.cloudflare.com/) and follow these simple steps. 

1. Change your name servers to [CloudFlares Nameservers](https://support.cloudflare.com/hc/en-us/articles/205195708-Changing-your-domain-nameservers-to-Cloudflare).
2. Make sure all your DNS records are migrated over to Cloudflare. 
3. Make sure Cloudflare is caching you site.  

You are ready to go! You have a professional custom blog with no monthly fees. 

Now I understand that this is not for everyone. If you would like to host a traditional blog you can run your it on [DigitalOcean](https://marketplace.digitalocean.com/apps/wordpress) for as little as $5 a month. You can still use cloudflares CDN to provide content delivery or use DigitalOcean [spaces](https://www.digitalocean.com/products/spaces/) to host static content which comes with built in CDN.

Have fun building!

---

## Like what you see?

Do not forget to folllow me on [twitter](https://twitter.com/_areyesjr) for updates and extras. 

<a href="../" class="button button--large">Back</a>