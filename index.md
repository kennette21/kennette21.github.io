---
layout: main
header: TBPortfolio
--- 
<h2>This is a list of Projects</h2>


<div class="explore-container">
{% for item in site.data.projects %}
    <a class="profile-topic wobble-vertical-on-hover" href="projects/{{item.name}}.html">
        {{ item.display-name }}
    </a>
{% endfor %}
</div>
