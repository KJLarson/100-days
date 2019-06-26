---
layout: post
title: "Day 23: State of the Web"
date: 2019-06-25
---

**Today's Progress:** Worked on my HTTP Archive's Almanac/State of the Web project again today. Worked on some of the suggested changes to my pull requests. I also worked on figuring out how we will organize the SQL queries in directories--not exactly coding, but still part of an open source project, so I'm counting it. 

This is what I'm thinking (I didn't fill in the whole thing, because there are a lot of files, but this should give the main idea):
```
sql
+--- 2019
|    +--- 01_JavaScript
|    |       01_01.sql
|    |       01_02.sql
|    +--- 02_CSS
|    |       02_01.sql
|    |       02_02.sql
|    |       02_03.sql
|    +--- 03_Markup
|    |       03_01.sql
|    |       03_02.sql
|    +--- 04_Media
|    |       04_01.sql
|    +--- 05_Third_Parties
|    |       05_01.sql
|    +--- 06_Fonts
|    +--- 07_Performance
|    +--- 08_Security
|    +--- 09_Accessibility
|    +--- 10_SEO
|    +--- 11_PWA
|    +--- 12_Mobile_Web
|    +--- 13_Ecommerce
|    +--- 14_CMS
|    +--- 15_Compression
|    +--- 16_Caching
|    +--- 17_CDN
|    +--- 18_Page_Weight
|    +--- 19_Resource_Hints
|    +--- 20_HTTP_2
+--- 2020
|    +--- 01_
```

The directories (no file extensions) correspond with the chapters of the Almanac. Each file will contain one query for a metric.

**Thoughts:** I had a rough start to the day, but working on this project helped my mood. I felt a lot more lively afterwards.

**Links to today's work:**
* [HTTP Archive's Almanac](https://github.com/HTTPArchive/almanac.httparchive.org)
  * [My forked repository](https://github.com/KJLarson/almanac.httparchive.org)