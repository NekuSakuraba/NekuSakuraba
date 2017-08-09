<head>
	<meta charset="utf-8">
	
	<title>
		{% if page.title %}
			{{ page.title | escape }}
		{% else %}
			{{ site.title[page.lang] | escape }}
		{% endif %}
	</title>
	
	<link rel="stylesheet" href="{{ "/css/style.css" | prepend: site.baseurl }}"> 
	
</head>