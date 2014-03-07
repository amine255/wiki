---
layout: default
---

<div class="row">
    {% for people in site.authors %}
        <div class="col-md-3">
        {% assign author = people[1] %}
            <img class="img-circle" src="http://www.gravatar.com/avatar/{{ author.gravatar }}?s=150" />
            <span class="flag-icon flag-icon-{{ author.nationality }}"></span>
            <h4> {{ author.display_name }}</h4>
            <ul class="list-inline">
                {% for ref in author.social %}
                    <li> <a href="http://www.{{ref.[0]}}.com/{{ref.[1]}}" target="_blank"> <i class="fa fa-{{ref.[0]}} fa-lg"></i></a> </li>
                {% endfor%}
            </ul>
        </div>
    {% endfor %}
</div>
