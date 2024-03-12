---
layout: page
title: news
nav: true
permalink: /news/
---


{% assign sorted = site.news | sort: 'date' | reverse %}
{% for news in sorted %}
  <div class="news">
    <ul>
      <article>
        <li> {{ news.date | date: "%b %d, %Y" }} {{ news.content }}  </li>
      </article>
    </ul>  
    </div>    
{% endfor %}
