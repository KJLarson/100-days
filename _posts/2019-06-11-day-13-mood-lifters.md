---
layout: post
title: "Day 13: Mood Lifters"
date: 2019-06-11
---

**Today's Progress:** Applying for jobs put me in a foul mood today, so I needed coding to be fun. I searched for cool JavaScript libraries, and came across [fartscroll.js](http://theonion.github.io/fartscroll.js/), made by the folks at The Onion. I had to try it, so I made a farting pen on CodePen (See link to work below). It makes me laugh so much! It wasn't hard to implement, but after I sent it to my sister I discovered it doesn't work on mobile. I spent some time trying to debug it, but couldn't figure out what was breaking it. 

After making the farting pen, I decided I wanted to make some art. I downloaded [Processing](https://processing.org/) a while ago, but hadn't done a whole lot with it yet. I spent some time looking at the tutorials and documentation, and then made this image with the word "ECHO" repeating itself.

![Screenshot of the word "ECHO" repeating 12 times]({{ site.baseurl }}/assets/echo-2019-06-11.png)

The code I used to make the ECHO art (Processing uses Java):

<pre>
<code class="processing">
size(400, 400);
background(220);

int x;
int y;
int num=12;

textSize(100);
fill(0, 140); // fill black with low opacity


x = 0;
y = 80;
for(int i = 0; i < num; i++) {
  text("Echo", x, y);
  if(i < 6){
    x+=20;
    y+=25;
  } else {
    x-=20;
    y+=25;
  }
}

save("echo.png");
</code>
</pre>


**Thoughts:** 'Twas a fun day coding. The farts crack me up.

**Links to work:** 

<p class="codepen" data-height="400" data-theme-id="0" data-default-tab="result" data-user="KariJL" data-slug-hash="xobEqE" style="height: 400px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Fart Scroll">
  <span>See the Pen <a href="https://codepen.io/KariJL/pen/xobEqE/">
  Fart Scroll</a> by Kari (<a href="https://codepen.io/KariJL">@KariJL</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>