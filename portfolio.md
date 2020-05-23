---
layout: main
header: TBPortfolio
permalink: /
--- 
<h2>This is a list of Projects</h2>
<!-- keeping this aruond because it was short and sweet-->
<!-- {% for item in site.data.projects %}
[{{item.display-name}}]({% link projects/{{item.name}}.md %})
{% endfor %} -->


<div class="explore-container">
{% for item in site.data.projects %}
    <a class="profile-topic wobble-vertical-on-hover" href="projects/{{item.name}}.html">
        {{ item.display-name }}
    </a>
{% endfor %}
</div>
