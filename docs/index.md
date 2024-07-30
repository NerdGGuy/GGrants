# Approved Grants

{% for grant in site.pages %}
  {% if grant.path contains 'approved_grants/' %}
    ## [{{ grant.title }}]({{ grant.url | relative_url }})
    {{ grant.content | truncate: 200 }}
    [Read more]({{ grant.url | relative_url }})
  {% endif %}
{% endfor %}
