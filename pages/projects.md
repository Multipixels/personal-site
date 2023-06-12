---
layout: page-fullwidth
title: "Projects"   
permalink: "/projects/"
---

<div class="medium-block-grid-3">
    {% for post in site.categories.projects %}
        <li>
            <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">
                <div width="100%">
                    <div style="position:relative; display: block; padding-bottom: 56.2%;">
                        {% if post.image.thumb %}
                            <img style="position: absolute; object-fit: cover; width: 100%; height: 100%;" src="{{ site.urlimg }}{{ post.image.thumb }}" alt="">
                        {% else %}
                            <img style="position: absolute; object-fit: cover; width: 100%; height: 100%;" src="https://upload.wikimedia.org/wikipedia/commons/0/07/Emperor_Penguin_Manchot_empereur.jpg" alt="">
                        {% endif %}
                    </div>
                    {{ post.title }}
                </div>
            </a>
            {% if post.teaser %}
                <p> {{ post.teaser }} </p>
            {% endif %}
        </li>
    {% endfor %}
</div>
