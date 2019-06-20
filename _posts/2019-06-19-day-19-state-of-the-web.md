---
layout: post
title: "Day 19: State of the Web (The Web Almanac)"
date: 2019-06-19
---

**Today's Progress:** Today, I worked more on the code for the Contributors page of The Web Almanac. I got some helpful feedback from other members of The Almanac team, and Rick gave me a brief list of the parts needed to get the data to the webpage (as well as some examples to look at). I came up with the following code, but I still want to do a little more work on it. Just not today, because I'm tired and think I need to step away from it for a bit. I might add the code to my working branch of the repository yet tonight, but I'm not sure yet.

Example of the layout of the JSON file that will store the contributor data:
<pre><code>
{
  "contributors": [
    { 
      "name": "John Doe",
      "teams": "Developer",
      "github": "github.com"
    },
    { 
      "name": "Sara Smith",
      "teams": "Analyst",
      "github": "github.com"
    }
  ]
}
</code></pre>

Using Python to grab the JSON data:
<pre><code>
import json

contributors_json = {}

with open('path to contributors.json') as contributors_file:
  contributors_json = json.load(contributors_file)
</code></pre>

Passing the data map to the Flask template:
{% raw %}
<code><pre>
import reports as report_util
from flask import jsonify

&#64;app.route('path to contributors.html')
  reports = report_util.get_reports()

&#35;return as JSON
if get_format(request) == 'json':
  return jsonify(name=contributors.name, teams=contributors.teams, etc)

return render_template('contributors.html', name=contributors.name, teams=contributors.teams, etc)
</code></pre>
{% endraw %}
Template for the UI (includes iterating through the data):
{% raw %}
<pre><code>
{% extends "en/base.html" %}

{% block title %}
  Contributors
{% endblock %}

{% block navigation %}{% endblock %}

{% block main %}
  {% for contributor in contributors %}
    &lt;section&gt;
      &lt;ul&gt;
        &lt;li&gt;{{ contributor.name }} <!-- or {{ name }} ? -->
          &lt;ul&gt;
            &lt;li&gt;{{ contributor.teams }}&lt;/li&gt; <!-- or {{ teams }} ? -->
            &lt;li&gt;{{ contributor.github }}&lt;/li&gt; <!-- or {{ github }} ? -->
            &lt;li&gt;{{ contributor.twitter }}&lt;/li&gt; <!-- or {{ twitter }} ? -->
          &lt;/ul&gt;
        &lt;/li&gt;
      &lt;/ul&gt;
    &lt;/section&gt;
  {% endfor %}
{% endblock %}
</code></pre>
{% endraw %}


**Thoughts:** This has been a good experience so far.

**Links to work:**

Haven't put my code online yet, but here are the repositories it will go to:
(I'm not sure if I need to share the original repository and my forked repository, so here are both of them just in case):
* [HTTP Archive's Almanac](https://github.com/HTTPArchive/almanac.httparchive.org)
  * [My forked repository](https://github.com/KJLarson/almanac.httparchive.org)

