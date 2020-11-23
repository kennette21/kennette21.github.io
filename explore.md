---
layout: main
header: TBExplore
---

<div class="portfolio-container">
    <div class="active-projects-list">
        {% for item in site.data.explore-topics %}
            {% unless item.hidden %}
                <a class="topic portfolio" href="explores/{{item.name}}.html">
                    {{ item.name }}
                </a>
                <div class="separator"></div>
            {% endunless %}
        {% endfor %}
    </div>
</div>