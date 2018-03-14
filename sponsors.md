---
title: Our Sponsors
layout: landingpage
# Future use, show this as what we offer to potential sponsors
benefits:
  - A shoutout at events
  - The ability to hand out marketing materials at the event
  - A spot on this site
---

<main role="main">
    <div class="container">
        <h1>Sponsors</h1>
        <div class="row">
            Our sponsors mean a lot to us, as they help shape what we're able to do at events. Feel free to check them out.
        </div>
        <hr />
        <div class="row">
            {% for sponsor in site.sponsors %}
                {% include component/summary.html summary=sponsor %}
            {% endfor %}
        </div>
    </div>
</main>
