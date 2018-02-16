# CSF
Django cache static files version


1. add cache_bust.py to your templatetags
2. in template load tag  {% load cache_bust %}
3. after your script add ?{% cache_bust %}

example:  <script src="{% static 'js/main.js' %}?{% cache_bust %}" type="text/javascript"></script>
4. in setings.py add PROJECT_VERSION = "1.001"

Than when you need refresh scripts for all users just change project version
