```
{% for link in links %}
    {% if link.rel == 'canonical' %}
        {% set new_href = link.href|replace({'': ''}) %}
        <link href="{{ new_href }}" rel="{{ link.rel }}" />
    {% else %}
        <link href="{{ link.href }}" rel="{{ link.rel }}" />
    {% endif %}
{% endfor %}
