---
layout: post
title: "Day 25: State of the Web (The Web Almanac)"
date: 2019-06-27
---

**Today's Progress:** I think it's almost time to merge my pull requests into the master branch of HTTP Archive's repository!

I made a few more changes to the code and did some trouble-shooting today. When I tried testing everything in a local environment, it wouldn't work. The first time I tried there was an error, and I was able to figure out this one by myself: the name of a utility we were trying to use didn't match what we called it on import.

We imported: `contributors_util`
We returned: `contributor_util` 
That doesn't work!!!

After this, the page loaded, but it was completely blank. I couldn't figure this one out on my own, so [Rick](https://github.com/rviscomi) helped. He sent me step-by-step instructions about how he solved the problem.

I tried recreating his steps, but was having issues and was getting an error saying a particular file didn't exist. I know it did, and I checked the spelling and the path a thousand times. I ended up adding the `src/` directory to the beginning of the path to make it work and I finished following Rick's debugging steps.

**The page worked!!!! Yay!!!!**

It turns out, when I started the local server, I wasn't inside the `src` directory, which is where it should be run from. I tried it from there, and then the code worked without `src/` at the beginning of the file path.

**Thoughts:** I'm starting to feel a little more comfortable using Git and GitHub. It was kind of scary at first, but it's getting easier.

I'm beginning to feel like a real developer because of this project!

**Links to today's work:**
* [HTTP Archive's Almanac](https://github.com/HTTPArchive/almanac.httparchive.org)
  * [My forked repository](https://github.com/KJLarson/almanac.httparchive.org)