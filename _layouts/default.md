<!DOCTYPE html>
<html>
　<head>
　  <meta http-equiv="content-type" content-type="text/html; charset=utf-8" />
    <link href="/assets/css/bootstrap.min.css" rel="stylesheet" type="text/css" media="screen">
    <link href="/assets/css/style.css" rel="stylesheet" type="text/css"  media="screen">
　　<title>{{ page.title }}</title>
　</head>
　<body>
    <div class="container-fluid">
      <div class="row-fluid">
        <div class="span10">
          {{ content }}
        </div>
        <div class="span2">
          <div id="search">
            <script>
              (function() {
               var cx = '003301499565717175039:boct6bawcwa';
               var gcse = document.createElement('script');
               gcse.type = 'text/javascript';
               gcse.async = true;
               gcse.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//www.google.com/cse/cse.js?cx=' + cx;
               var s = document.getElementsByTagName('script')[0];
               s.parentNode.insertBefore(gcse, s);
              })();
            </script>
            <gcse:search></gcse:search>
          </div>
          <div id="category">
            <h4>Category</h4>
            <ul>
              {% for category in site.categories %}
              <li><a href="/categories/{{ category | first }}/index.html" title="view all posts">{{ category | first }} {{ category | last | size }}</a></li>
              {% endfor %}
            </ul>
          </div>
          <div id="tag">
          <ul class="tag_box inline">
              {% for tag in site.tags %}
              <li><a href="/tags/{{ tag | first }}/index.html" title="view all posts">{{ tag | first }} <span>{{ tag | last | size }}</span></a></li>
              {% endfor %}
          </ul>
        </div>
      </div>
    </div>
　</body>
</html>
