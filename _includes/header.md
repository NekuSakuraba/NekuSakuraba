<header class="site-header">
  <div class="wrapper">

    <a class="site-title" href="{{ site.baseurl }}/{{ site.index[page.lang] }}">{{ site.title[page.lang] }}</a>

    <nav class="nav">
		<ul>
			<li></li>
			<li>Quem sou eu?!</li>
			<li class="lang">
				{% assign posts=site.posts | where:"ref", page.ref | sort: 'lang' %}
				{% for post in posts %} <a href="{{ post.url | prepend: site.baseurl }}" class="{{ post.lang }}">{{ post.lang }}</a> {% endfor %}

				{% assign pages=site.pages | where:"ref", page.ref | sort: 'lang' %}
				{% for page in pages %} <a href="{{ page.url | prepend: site.baseurl }}" class="{{ page.lang }}">{{ page.lang }}</a> {% endfor %}
			</li>
		</ul>

	<div class="wrapper" style="text-align: right; line-height: 2em; z-index: -1; position:relative;">
	</div>
	  
    </nav>

  </div>
</header>

