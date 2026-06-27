<!doctype html>
<html>
  <head>
     <link rel="stylesheet" href="/assets/css/main.css"> 
    <meta charset="utf-8">
    <title>{{ page.title }} | {{site.title}}</title>
  </head>
  <body>
    <div class="container-fluid" style="padding-top: 1%; padding-bottom: 70px;">
      {{ content }}
    </div>
    {% include navbar.html %}
    <script src='/assets/js/main.js'><script/>
  </body>
</html>