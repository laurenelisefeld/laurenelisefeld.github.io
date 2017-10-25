---
layout: post
title:      "My CLI Data Project Journey"
date:       2017-10-24 11:01:33 -0400
permalink:  cli_data_gem_portfolio_project
---

![](https://i.pinimg.com/originals/a2/9a/bc/a29abc6432badfba5106344c11c88029.jpg)

Phew! Is it really over? What a journey it has been. While reading through the requirements for the project I was a tad concerned that i would not be able to put all the material together and create my own CLI program. After spending a fair amount of time searching for scrapable websites, I finally found one that was able to scrape but I had to make a few minor adjustments. With much reseach, I discovered that I had to add 'amp' to the beginning of the site's url to access the accelerated mobile page version of the website. This was because the page was loading everything except the first item on the line using JQuery, which only allowed my scraper access to the very first selector (and thus restaurant) on the page.

Once that issue was resolved, I started to see the light at the end of the tunnel. My page became easier to scrape! Later down the road, I came across another issue. When It came to finding the right selectors to grab my desired text, I had to change the selector that I was using for the name of the pizza restaurent I was scraping because it was not nested under the same DIV. Took a little bit of time to figure this out, but I perservered! 

**MOVING ON!....**... While creating my attributes I had to refer back to the Regex lab and use Rubular to brush up on regular expressions. This was because I needed to use regex a few times since the page wasn't breaking everything down into the desired divs for me to iterate over, so I was iterating over a large block of text inside a "p" selector. As a result, I was having the same issue when trying to pull each restaurant name. To solve this problem, I had to create a separate method just to scrape the name, and it was a bit of a challenge figuring out how I could get that added into my object array of restaurants. I ended up calling it directly from the CLI itself, probably not the most elegant solution, but it was the best solution I found, and it works!

![](httphttps://i.pinimg.com/originals/17/26/5e/17265e343ef9d45141666427cbb085f0.jpg://)





