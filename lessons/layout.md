# Layout

In mean there are a couple of places we can control the layout

### Node based layout

packages/core/system/server/views/index.html

```
{% extends 'layouts/default.html' %}
{% block content %}
  <section data-ui-view ></section>
  <script type="text/javascript">
    window.user = {{user|json|safe}};
    window.modules = null;
  </script>
{% endblock %}
```
packages/core/system/server/views/index.html
```
<!doctype html>
<html lang="en" xmlns="http://www.w3.org/1999/xhtml" xmlns:fb="https://www.facebook.com/2008/fbml" itemscope="itemscope" itemtype="http://schema.org/Product">
{% include '../includes/head.html' %}

<body data-ng-controller="ThemeController" ng-cloak class="ng-cloak" ng-class="state">
    <!-- {% include '../layouts/header.html' %} -->
    <div class="navbar navbar-inverse navbar-fixed-top" data-ng-include="'/system/views/header.html'" data-role="navigation"></div>
    <div data-ng-include="'/admin/views/index.html'"></div>
    <section class="content">
        <section class="container">
            {% block content %}{% endblock %}
        </section>
    </section>
    {% include '../includes/foot.html' %}
</body>

</html>
```
* file server/includes...


### Angular layout

* ng-include based stuff


