---
layout: list
---

Krótka notatka od <a href="/ksp/about.html">starego pryka</a>

<h3>Kierowniku, w czym pomóc?</h3>

{% assign gamesList = site.data.games.list | sort: 'title' %}
<ol>
	{% for game in gamesList %}
		<li><a href="/ksp/game/{{ game.file }}.html" alt="{{ game.title }}">{{ game.title }}</a></li>
	{% endfor %}
</ol>
