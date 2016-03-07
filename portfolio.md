---
layout: page
title: Portfolio
permalink: /portfolio/
---

<div class="container">
    <!-- Example row of columns -->
    <div class="row work">
        <ul>
            {% for post in site.posts %}
            <li>
                <div class="col-sm-6 col-md-4">
                    <div class="thumbnail hvr-box-shadow-outset">
                            {% if post.image %}
                            <a href="{{ post.url }}"><img src="../img/{{ post.image }}" alt="..."></a>
                            {% endif %}
                            <div class="caption">
                                <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
                                <p>{{ post.description }}</p>
                            </div>
                    </div>
                </div>
            </li>                            
            {% endfor %}
        </ul>
    </div><!-- row work-->
</div>