---
title: "Mery"
layout: default
permalink: "/author-mery"
---
<div class="container">
<div class="row justify-content-center">
    <div class="col-md-8">        
        <div class="row align-items-center mb-5">
            <div class="col-md-9">
                <h2 class="font-weight-bold">{{page.title}} <span class="small btn btn-outline-success btn-sm btn-round"><a href="{{ site.authors.Mery.twitter }}">Follow</a></span></h2>
                <p><a href="{{ site.authors.Mery.site }}">{{ site.authors.Mery.site }}</a></p>
                <p class="excerpt">{{ site.authors.Mery.bio }}</p>
            </div>
            <div class="col-md-3 text-right">
                <img alt="{{ site.authors.sal.name }}" src="{{site.url}}/{{ site.authors.Mery.avatar }}" class="rounded-circle" height="100" width="100">
            </div>
        </div>
        <h4 class="font-weight-bold spanborder"><span>Posts by {{page.title}}</span></h4>
            {% assign posts = site.posts | where:"author","Mery" %}
            {% for post in posts %}
            {% include main-loop-card.html %}
            {% endfor %}
    </div>
</div>
</div>
