
<H2>Images</H2>

{% for file in site.static_files %}
  {% if file.path contains "/images/" %}
    {% if file.extname == ".png" or file.extname == ".PNG" or file.extname == ".ico" or file.extname == ".svg" %}
* [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
    {% endif %}
  {% endif %}
{% endfor %}


<style>
ul > li > p {
  margin: 0 0 0px;
}
</style>
