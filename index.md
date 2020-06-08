---
layout: main
header: TBPortfolio
--- 
<h2>This is a list of Projects</h2>


<div class="portfolio-container">
    <div class="active-projects-list">
        {% for item in site.data.projects %}
            {% if item.status == "development" %}
                <a class="topic profile  wobble-vertical-on-hover" href="projects/{{item.name}}.html">
                    {{ item.display-name }}
                </a>
            {% endif %}
        {% endfor %}
    </div> 
    <div class="separator"></div>  
    <div class="dormant-projects-list">
        {% for item in site.data.projects %}
            {% if item.status == "dormant" %}
                <a class="topic profile dormant wobble-vertical-on-hover" href="projects/{{item.name}}.html">
                    {{ item.display-name }}
                </a>
            {% endif %}
        {% endfor %}
    </div>
</div>
