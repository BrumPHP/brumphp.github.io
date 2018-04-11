---
title: BrumPHP
layout: landingpage
---

<main role="main">
    <div class="jumbotron mb-0">
        <div class="container">
            <h1 class="display-3">BrumPHP</h1>
            <p>
                We are starting on a mission to showcase, discuss and learn anything in the world of PHP Developer life, encompassing anything from Symfony and Laravel, Composer, Personal/Commercial app demos, Toolchains, Dev culture and of course, Birmingham.
                <br/>
                Don't hesitate to <a href="/community">get in touch</a> if there is a subject or idea you'd like to discuss!
            </p>
        </div>
    </div>
</main>
<section class="brum--bg--yellow brum--fg--white">
    <div class="container">
        {% assign nextEvent = site.events.last %}
        <p class="py-4">Next meetup: <a class="py-4" class="brum--fg--navy-blue" href="{{nextEvent.link}}">{{nextEvent.date | date: "%a %b %d %Y"}} at {{nextEvent.location}}</a></p>
    </div>
</section>
<section>
    <div class="container pb-2">
        <h2>Events</h2>
        <div class="row">
            {% for event in site.events reversed limit:3 %}
                {% include component/summary.html summary=event %}
            {% endfor %}
        </div>
    </div>
</section>
