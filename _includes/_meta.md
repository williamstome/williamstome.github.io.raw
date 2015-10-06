<style media="screen" type="text/css" >

.meta-wrapper{
		border: 1px solid #888;
		border-width: 2px 0;
		color: #4e4e4e;
		text-transform: uppercase;
		margin: 0px 0px 20px 0px
}

.inline{display:inline}

.tag_list_in_post{
	display: inline;
	padding: 0 0 0 30px;
}


.tag_list{
	padding-bottom: 50px;
}

.tag_list_item{
	font-family: "PT Sans Narrow",sans-serif;
}
	
.tag_list_link{
	color: #4e4e4e;
	font-size: 18px;
	font-variant: small-caps;
	padding: 0 6px;
	text-transform: lowercase;
}

.tag_list_link:hover{
	color: #888;
}
</style>

<div class="meta-wrapper">
<ul class="tag_list_in_post">
{% for tag in page.tags %}
<li class="inline tag_list_item">
<a class="tag_list_link" href="/tag/{{ tag }}"> {{ tag }} </a>
</li>
{% endfor %}
</ul>
</div>
