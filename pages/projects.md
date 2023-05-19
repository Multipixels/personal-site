---
layout: page-fullwidth
title: "Projects"   
permalink: "/projects/"
---

<div class="medium-block-grid-3">
    {% for post in site.categories.projects %}
        <li>
            <a href="{{ post.url }}">
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
        </li>
    {% endfor %}
</div>


<!-- <div class="row">
    <div class="medium-4 columns ">
        <img src="{{ site.urlimg }}webdesign_screenshot_andersneu.jpg" alt="">
        <p>Website: <a href="https://andersneu.de/">andersneu.de</a></p>
    </div>

    <div class="medium-4 columns ">
        <img src="{{ site.urlimg }}webdesign_screenshot_mosonic.jpg" alt="">
        <p>Website: <a href="https://mosonic.net/">mosonic.net</a></p>
    </div>

    <div class="medium-4 columns ">
        <img src="{{ site.urlimg }}webdesign_screenshot_moritz_sauer.jpg" alt="">
        <p>Website: <a href="https://moritz.sauer.io/">Webdesign, SEO, Music</a></p>
    </div>
</div> -->

