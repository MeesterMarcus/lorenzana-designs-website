---
layout: post
title: Top 5 Methods To Make Your Website FAST
date: 2020-09-22T09:56:39.000+00:00
categories:
- webdesign
comments: true

---
Is your website running slower than usual, or has it always just been irritatingly sluggish to load? You're not alone! Tuning your WordPress, Joomla, or static website can be a daunting task. Especially if you have a lot of content on your website. Read on to learn about the top 5 methods you can increase the usability and speed of your website and increase customer retention! I don't know about you, but whenever I land on a page that takes more than 5 seconds to load, I'll move on. In this day and age, with rapid information being relayed to the user on a daily basis, we have shorter attention spans and the need for SPEED.

<img src="/assets/img/posts/5-methods-fast/1.jpeg">
<h3>Method #1: Optimize your images</h3>

One of the major issues I run into a lot with my clients is poor image optimization. Having larger images than necessary or large file sizes can bring your website to a crawl. You can see this in action if you open up dev tools in your browser and monitor the network tab and see which images are the biggest abusers. So how do you fix it? There are a couple of relatively easy ways but can take time if you have a lot of images. The first and most obvious method is to reduce the size of the image. This can be done by both compressing the image and reducing the resolution. I see many websites sometimes use 4k images for banners on websites or as a background image for section header that wreck the website's performance. This is unnecessary, and reducing the resolution / compressing will result in the same look and feel at a faster response. Another method is to use images that are optimized specifically for the web; this includes formats such as SVG or WEBP. The great thing about SVG images is that it can scale to any device size and retain its quality if implemented correctly. Finally, one great tool I like to use that is free and easy is BIRME, which allows reducing images resolution and size in bulk: [https://www.birme.net/](https://www.birme.net/ "https://www.birme.net/")

<img src="/assets/img/posts/5-methods-fast/2.jpeg">
<h3>Method #2: Switch or upgrade your hosting</h3>

An often-overlooked reason why a website could be slow is a poor hosting provider or choosing the wrong tier of hosting. When they start out, many businesses go with the cheapest option to get their website live, not taking into account growth and bandwidth. If you are a small business just starting, you can get away with this, and it probably makes more sense. But as your business grows and more traffic goes to your website, you'll need to upgrade your hosting. Upgrading your hosting will allow for greater bandwidth, the ability to load your website for larger audiences at once, and give priority over lower-tier hosting websites. This is especially true if you go from shared hosting to a dedicated server for your website.

<img src="/assets/img/posts/5-methods-fast/3.png">
<h3>Method #3: Monitor your API calls / Choose the right plugins</h3>

Another way you can increase your website's speed is by ensuring that you are calling APIs or using quick plugins. If you use the network tab in dev tools, you'll see there are usually many requests, some taking significantly longer than others. This can be fixed by making sure you call an API that is fast and can handle multiple requests. If you are using WordPress, then make sure you are using plugins that are well optimized. This may take trial and error, finding the right ones.

<img src="/assets/img/posts/5-methods-fast/4.jpeg">
<h3>Method #4: Minify your vendor files</h3>

A great way to speed up your website is to ensure that the vendor files you are using are minified. What does minified mean? This essentially means to reduce the size of your JS and CSS files that you use from various sources or vendors. A large majority of the time, the vendor has a version of their library or plugin that is "minified." This can be seen by the extension of the file. For example, with bootstrap, you could use either bootstrap.js or bootstrap.min.js. Using the latter will improve the performance of using that framework. If you are using WordPress, you can use a general-purpose minify plugin such as this:
Fast Velocity Minify
Improve your speed score on GTmetrix, Pingdom Tools and Google PageSpeed Insights by merging and minifying CSS…
wordpress.org

<img src="/assets/img/posts/5-methods-fast/5.jpeg">
<h3>Method 5: Caching and CDNs</h3>

Last but not least, using caching and CDN's on your website will improve your website performance enormously. What caching essentially does is store assets from a website in temporary storage, which allows the user to load the website MUCH quicker the next time they visit. This is especially useful for repeat visitors to your website. Here is a WordPress plugin that will handle this for you with some basic configuration:
W3 Total Cache
W3 Total Cache (W3TC) improves the SEO and user experience of your site by increasing website performance and reducing…
wordpress.org
In addition to caching, using CDNs in your website will greatly improve speed as well. This will reduce the latency of your website by loading your site's content on various servers and when a user visits your page, it will find the server closest to them. For instance, if you live in San Antonio, TX, but your hosting provider's server is located in New York, you'll experience significantly higher latency than if the server is located in, say, Houston. Signing your website up for a CDN is a great way to ensure that your website's content is served FAST and with very low latency. In my opinion, however, I would only explore this option once you have gone through the above and you are still experiencing a slowdown.

<h3>Summary</h3>

Thank you guys for reading my article, and I hope it will help speed up your website! Don't forget to use a tool like Google's PageSpeed Insights to check the before and after and see the difference. It will also help offer suggestions for you, such as the ones above and rank the suggestions in what would help you out the most!