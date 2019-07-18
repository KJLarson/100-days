---
layout: post
title: "Day 32: Windows PowerShell"
date: 2019-07-17
---

**Today's Progress:** I worked more with PowerShell at work today. After getting the file counts working yesterday, I decided it would be nice to also know the size of each directory. I did some research and found a guest blog by [Bill Stewart](https://devblogs.microsoft.com/scripting/getting-directory-sizes-in-powershell/). His script worked quite beautifully, but there were a few changes I wanted to make:
* Display the folder sizes with commas separating the thousands
* Recurse into all of the folders in the directory tree
* Export data to a CSV file (the results of the code just show in PowerShell)

I don't know PowerShell too well, so I looked up what different parts of the code mean and what they're supposed to do. I tried making changes, but ultimately I was unable to accomplish any of the things I wanted to.

Apparently, the code was already supposed to format the numbers, but that didn't happen when I ran it. The article was written in 2012, so I suppose the changes to PowerShell since then could have broken that bit of the code. I tried changing the [number format specifiers](https://devblogs.microsoft.com/scripting/use-powershell-and-conditional-formatting-to-format-numbers/), but that didn't do anything.

When I've worked with PowerShell in the past, simply adding a `-Recurse` parameter has always been enough to do what I needed. This code is more complicated than I'm used to, with some extra stuff added in. Some of the changes I tried in regard to the recurse parameter had some unexpected results, so I will need to investigate further.

I know how to export CSV files in PowerShell, but had problems figuring out where I needed to place the `Export-Csv` bit of code. There were some places I tried where it wouldn't export anything, and others where it would only export one line of data. I'm wondering if there are multiple places I need to add the code, as there are multiple `if-else` statements and `for` loops, so maybe I need to capture results from all the pieces separately. I didn't try that yet...

**Thoughts:** I know enough about PowerShell and programming (like `if-else` statements, `for` loops, etc.) that I understand the big picture of what this code is doing. It's the smaller details and PowerShell syntax that are throwing me off with this project. This script I was working with was quite large, and so I wasn't able to look up every piece of it to understand the finer details, at least not in one work day. I'll probably continue to try to figure it all out.

**Links to today's work:** No links to my work today
