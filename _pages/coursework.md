---
layout: page
title: coursework
permalink: /coursework/
display_categories: [Computer Science, Mathematics]
horizontal: false
nav: true
---

> Highlight courses that I've taken so far at Stanford.
<div class="coursework">
{%- for subject in page.display_categories %}
    <h1 style="font-weight:bold;"> {{subject}} </h1>
    <div class="course" style="padding: 10px;">
    {%- for course in site.data.courses[subject] %}
    <div class="course" style="padding: 10px;">
        {% assign courseName = course[0]%}
        <h2> {{courseName}} </h2>
        {%- for info in course[1] %}
            {% assign courseCode = info["code"]%}
            {% assign courseTitle = info["title"]%}
            {% assign courseYear = info["year"]%}
            <h4> {{courseCode}} | {{courseTitle}} | {{courseYear}} </h4>
        {%- endfor %}
    </div>
    {%- endfor %}
    </div>
{%- endfor %}
</div>