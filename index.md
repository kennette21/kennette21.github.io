---
layout: main
header: TBPortfolio
--- 

<div class="portfolio-container">
    <div class="active-projects-list">
    <div class="separator"></div>
        {% for item in site.data.projects %}
            <a class="topic profile " href="projects/{{item.name}}.html">
                {{ item.display-name }}
            </a>
            <div class="separator"></div>
        {% endfor %}
    </div>
</div>
