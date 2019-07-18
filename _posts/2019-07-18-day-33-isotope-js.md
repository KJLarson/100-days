---
layout: post
title: "Day 33: Food Opinions with Isotope.js"
date: 2019-07-18
---

**Today's Progress:** I returned to my CodePen project from Day 30, where I used Isotope.js to filter a bunch of food images. It wasn't working then, but I fixed it today!

I compared my Pen with the example Pen from the Isotope page, and after about 10 or so minutes, I found the problem.

I had left out part of the line where I defined the grid. Here's my non-working version:

```javascript
// Init Isotope
$('.grid').isotope({
  // options
  itemSelector: '.grid-item'
});
```

Here's what I changed it to in order for it to work:
```javascript
// Init Isotope
var $grid = $('.grid').isotope({
  // options
  itemSelector: '.grid-item'
});
```


<svg class="ta-da" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 122.88545 114.88568" style="width: 65px; height: 65px; display: inline-block">
 <g fill="#fff" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.7613" transform="matrix(.72428 0 0 .72428 -122.55 -265.22)">
  <path d="m249.29 389-9.7738 30.16-31.92 7.5995c-2.7468 1.4659-5.5124 2.9244-1.6985 6.9998l30.159 12.578-11.809 32.074c-1.5695 4.6228-0.21957 6.3616 4.2421 3.3542l26.592-24.557 30.958 17.759c3.8332 2.6589 6.1209 0.80055 5.3635-3.5714l-12.107-34.118 22.726-13.707c2.328-1.034 5.8555-6.1605-0.46651-6.4604l-33.501-0.66887-11.696-27.262c-2.0428-3.5058-4.066-7.2275-7.0682-0.1801z"/>
  <path d="m170.58 468.2 34.362-7.3634"/>
  <path d="m256.49 486.61 2.4545 36.817"/>
  <path d="m304.35 448.57 33.135 1.2272"/>
  <path d="m284.72 398.25 23.317-30.681"/>
  <path d="m197.58 374.93 22.09 24.545"/>
 </g>
</svg><p class="ta-da">Ta-Da!!!</p><svg class="ta-da" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 122.88545 114.88568" style="width: 65px; height: 65px; display: inline-block">
 <g fill="#fff" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.7613" transform="matrix(.72428 0 0 .72428 -122.55 -265.22)">
  <path d="m249.29 389-9.7738 30.16-31.92 7.5995c-2.7468 1.4659-5.5124 2.9244-1.6985 6.9998l30.159 12.578-11.809 32.074c-1.5695 4.6228-0.21957 6.3616 4.2421 3.3542l26.592-24.557 30.958 17.759c3.8332 2.6589 6.1209 0.80055 5.3635-3.5714l-12.107-34.118 22.726-13.707c2.328-1.034 5.8555-6.1605-0.46651-6.4604l-33.501-0.66887-11.696-27.262c-2.0428-3.5058-4.066-7.2275-7.0682-0.1801z"/>
  <path d="m170.58 468.2 34.362-7.3634"/>
  <path d="m256.49 486.61 2.4545 36.817"/>
  <path d="m304.35 448.57 33.135 1.2272"/>
  <path d="m284.72 398.25 23.317-30.681"/>
  <path d="m197.58 374.93 22.09 24.545"/>
 </g>
</svg>

**Thoughts:** So fun. I was having just a bit of a slump in terms of coding every day. This was a fun project, so hopefully it will help me get back into the game!



**Links to today's work:** 

<p class="codepen" data-height="593" data-theme-id="0" data-default-tab="result" data-user="KariJL" data-slug-hash="rXNRLO" style="height: 593px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Food Opinions">
  <span>See the Pen <a href="https://codepen.io/KariJL/pen/rXNRLO/">
  Food Opinions</a> by Kari (<a href="https://codepen.io/KariJL">@KariJL</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>