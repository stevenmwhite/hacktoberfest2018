---
layout: landing
---

# We thought we'd update this site for 2020, and here's those of us who participated!

{% assign participantTwenty = site.participants | where: 'hf2020', 'participated' %}
{% for participant in participantTwenty %}
<li>
    <h2>
        <a href="{{ site.baseurl}}/{{ participant.url }}">
            {{ participant.name }}
        </a>
    </h2>
    <a href="{{ site.baseurl}}/{{ participant.url }}">
        <img src="https://github.com/{{ participant.github_username }}.png">
    </a>
</li>
<br><br>
{% endfor %}

# Find out more about a bunch of us who participated in Hacktoberfest 2018!

{% assign participantEighteen = site.participants | where: 'hf2018', 'participated' %}
{% for participant in participantEighteen %}
<li>
    <h2>
        <a href="{{ site.baseurl}}/{{ participant.url }}">
            {{ participant.name }}
        </a>
    </h2>
    <a href="{{ site.baseurl}}/{{ participant.url }}">
        <img src="https://github.com/{{ participant.github_username }}.png">
    </a>
</li>
<br><br>
{% endfor %}