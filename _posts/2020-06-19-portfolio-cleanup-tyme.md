---
layout: post
author: tom
tags: portfolio
---

# Simplify. 

The idea of having an interactive eye catching list. But as a first iteration, just have a good looking simple list. This way you can still show it off and say * ITS UNDER CONSTRUCTION *. I am not comfortable sending it out to potential employers as a professional description of myself, or to my peers as a personal description of myself.

### Build it simple first.
Steps to do that:
- single item list of links with brief description of the project.
- 

### In the future:
Actually impliment the dormant vs active separation.
```
*>||| in the html
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
```
```
*>||| in the main.sass
.active-projects-list {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-around;
  align-content: space-around;
}

.dormant-projects-list {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-around;
  align-content: space-around;
}

// todo: convert to topic parent and explore/profile children. same for container

.topic {
  display: flex;
  margin: 5px;
  justify-content: center;
  height: 140px;
  width: 140px;
  align-items: center;
  text-decoration: none;
  color: black;
  -webkit-transition: background-color .3s linear, color .2s linear;
  -ms-transition: background-color .3s linear, color .2s linear;
  transition: background-color .3s linear, color .2s linear;

  &.explore {
    border-radius: 70px;
    background-color: cornsilk;
    flex: 0 1 calc(20% - 8px);

    &:hover {
      background-color: cornflowerblue;
      color: white;
    }
  }

  &.profile {
    border-radius: 20px;
    background-color: lightgray;
    flex: 0 1 calc(30% - 8px);
    font-size: 16px;

    &:hover {
      background-color: gray;
      color: white;
    }
  }

  &.dormant {
    height: 80px;
    width: 80px;
    font-size: 12px;
    flex: 0 1 calc(15% - 8px);
  }
}

```
