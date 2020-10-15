---
layout: post
title: How to debug your website or web application without leaving the browser
date: 2020-09-27 17:00:00 +0000
categories: development
comments: false

---
Throughout all my experience as a Software Engineer and Web Designer, I’ve had the opportunity to work on a large amount of software and tools. And now with web development rapidly evolving and growing exponentially, more will continue to come.

There is one tool however, that is so easily available and so extremely useful that many developers overlook. It comes with almost all browsers and that’s the **dev tools**. I cannot begin to describe how much I use the dev tools / console for debugging and testing things out real time. I firmly believe that all web developers and web designer should have a solid grasp of it as it will make your life so much easier. Almost all of these methods below will apply with slight variation on all widely used browsers. For this guide however, I’m going to focus on Chrome dev tools as I am most familiar with it and the browser of choice for most people.

## Tip #1: The console

One of the most if not the most important aspect of Chrome Dev Tools is the console, which outputs all logging messages and JavaScript runtime messages. The first thing I do when a bug is brought up to me or I run into one myself and it is JavaScript related, is to check the console. A large majority of the time it will spit out exactly what is wrong such as a missing file, missing dependency, image, etc. and can be rectified quite easily. Another useful thing you can do in the console is to actually write JavaScript code inline and test various functionality. I don’t do this very often but it is good to know.

Here is a great example of how a small typo can completely crash your whole website leaving you dumbfounded as to where it is occurring. With the console however, it is very easy to detect what went wrong:

![](/uploads/1.jpeg)

You can see here that there is an Uncaught TypeError on line 17 on the main.js file. If we click the link that leads to it we can see the problem:

![](/uploads/2.jpeg)

We forgot to add the ‘$’ sign at the beginning of the click event! After adding it, our console is clean and our app is back up and running.

## **Tip #2: Edit CSS Live with the Elements tab**

If you right click any element on a page and click “Inspect Element”, Chrome DevTools will take you to the code inside the HTML where you can inspect and edit. Depending on the HTML structure, you may not always get pointed exactly where you want it to be but it will take you to the general location and you can expand tags to see where you want to edit exactly.

In this example, I’ll mess with a CSS class and see what it looks like live. Then once I’m happy, I can it implement in the actual code and save it.

![](/uploads/3.jpeg)

Here I decided I wanted to see how different colors would look like or how the class is being built for the “Us” colored text. If I right click and inspect it, it takes me here. You’ll see on the left pane it shows where in the HTML it is located, and on the right pane we can see the CSS class associated with it. Let’s see what happens if I change the color to red:

![](/uploads/4.jpeg)

Now I can see on the live website how it would look without altering any of the actual code permanently! All without leaving the browser, leaving my place in the page, or having to refresh. I can’t begin to tell you how useful this is. This example is rather simple, but it is going to save you so much time I guarantee it!

## Tip #3: Network Tab

I live in this tab. A large amount of my JS debugging efforts happens here when I need to inspect HTTP requests that I am making to a server. What this tab will do is monitor all network traffic on the website, show how long each request takes, the order of the requests, how the response looks, the headers used to make the request, and more. Let’s check it out.

I’m going to go ahead and click the Network tab, and for what I want to debug right now I will click “XHR” which will look for all inbound and outbound API requests.

![](/uploads/5.jpeg)

If you see the image above, we can find all the requests that were made on load of the page. It’s important to note that you must have Chrome DevTools open **prior** to the calls being made in order for it to track this data and display it for you. Let’s go ahead and check the “countries” request:

![](/uploads/6.jpeg)

Awesome! We are getting a successful response. Most of the time I click the “Preview” tab when I want to see the response on the right pane in order to format the JSON better and able to navigate it easier. Here we can see how the data is coming back to us, how many records there are, and all the JSON objects in the array. We can expand the nested objects too. This is incredibly useful for debugging. In this case, we are using this data to be read by a autocomplete list. By looking at the data, especially if it is an API we are not familiar with, we can see how we want to plug it in our so that it reads it the way the request has the model laid out.

![](/uploads/1_n1ch2osrtphld96rtjruqw.jpeg)

## Summary

This only scratches the surface of what you can do with the Chrome DevTools. Another essential tool is the Debugger tab, which allows you to set breakpoints in the live code and either check if it is reaching it correctly, if the error occurs before or after it, or how the data looks at that specific point in time. And much more!

However, I hope this guide helps you get your feet wet and proves useful for your development. I may go over the Debugger in another blog post as it probably needs it’s own article. I do think that these tips will be quite useful though and are the ones I use most frequently with my debugging efforts.

Thanks again and stick around for more content! Also check out my business website if you are ever interested in consulting or need web development services here: [Lorenzana Web Design](https://www.lorenzanadesigns.com/) .