---
layout: main
header: TBPortfolio
--- 
<h2>This is a list of Projects</h2>
plz work
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
