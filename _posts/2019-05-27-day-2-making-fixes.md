---
layout: post
title: "Day 2: Making Fixes"
date: 2019-05-27
---

**Today's Progress:** Today, I made some fixes to my web portfolio. It had some responsiveness problems (some images and text were spreading past their boundaries on smaller screens) and I decided I wanted to make my navigation bar fixed to the top. 

With some research, I figured out how to include several versions of an image in different sizes using `<img srcset=””>`. I have my images saved in a [Cloudinary](https://cloudinary.com/) account, which makes it really easy to add multiple sizes. I also looked up how to make text responsive and discovered it can be really easy by using `vw` units rather than `px` or `em`. That was exciting. I didn't read too much into the details of `vw`, so I'm not sure if there are times when it's good to use it and/or times when it could be problematic (I wonder about it making text too small). I'll have to do more research.

The navbar I had on my site before today worked and looked fine, but I decided I wanted it to stay at the top of the page when users scroll. I tried just adding `position: fixed;` to the CSS, but that messed up the hamburger menu and drop down that show on smaller screens. So, I totally redid the navigation. Nav bars can still be a bit tricky for me sometimes, so I decided to find some examples online. I found one I liked, and then had to fit it into my project. I changed the links and then had to change the styling so that it would fit my site.

**Thoughts:** I've discovered (several times) that it's often easier to code your HTML from the beginning than it is to take some existing code and redo it. It can be hard to keep track of the changes you need to make, what you already did, and what bits of code are from the old stuff vs. the new changes. I tend to keep the old code and write the new stuff right below it, so I can reference the old stuff and have a cleaner working space than I would if I were just changing the code. Then I'll comment out the old stuff, make sure the new stuff works, and then if it does I can delete the old code. That seems to work well for me.

**Link to work:** [Web portfolio](https://www.kjlarson.com)
