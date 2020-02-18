---
layout: "page"
title: "Elecciones Latinoamerica"
date: 2020-02-17
---
<table>
		<tr>
			<td><h2>Elecciones 2020</h2></td>
		</tr>
		{% for election in site.elections %}
		<tr>
			<td>{{ election.country }}</td>
			<td><input type="button" onclick="location.href='{{ site.url }}elections/{{ election.name }}';" value="Ver Más" /></td>
		</tr>
		{% endfor %}
	</table>