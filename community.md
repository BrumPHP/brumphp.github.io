---
title: Community
layout: landingpage
community:
  -
    title: Meetup
    description: Join the meetup group for event announcements and updates!
    img: https://upload.wikimedia.org/wikipedia/commons/6/6b/Meetup_Logo.png
    link: https://www.meetup.com/brumphp/
    buttonText: Join the group
  -
    title: Twitter
    description: We like to shout about tech and Birmingham. Tweet us with questions and follow for updates.
    img: http://www.stickpng.com/assets/images/580b57fcd9996e24bc43c53e.png
    link: https://twitter.com/brumphp
    buttonText: Follow us
  -
    title: Slack
    description: "You can talk to us on the Brum Tech slack. We're the #brumphp channel."
    img: https://upload.wikimedia.org/wikipedia/commons/7/76/Slack_Icon.png
    link: https://upload.wikimedia.org/wikipedia/commons/7/76/Slack_Icon.png
    buttonText: Join the BrumTech Slack
---

<main role="main">
    <div class="container">
        <h1>{{page.title}}</h1>
        <div class="row">
            <div class="col-md-12">
                <p>
                    Here's 3 quick ways to get involved with the community. Any questions can sent via any of the following.
                </p>
            </div>
        </div>
        <hr />
        <div class="row">
            {% for item in page.community %}
                {% include component/summary.html summary=item %}
            {% endfor %}
        </div>
    </div>
</main>
