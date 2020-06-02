---
layout: page
---

Welcome to Zixuan's homepage, you can call me Vincent.
I'm currently a second year Master student at Johns Hopkins University. My major is Computer Science. I live in Baltimore, Maryland. For any question, please contact me through email: [yao@jhu.edu](mailto:yao@jhu.edu) or [yaozixuan0411@gmail.com](mailto:yaozixuan0411@gmail.com).

<iframe src="/resume.pdf" style="width:750px; height:970px;" frameborder="0"></iframe>

{%- if site.posts.size > 0 -%}
<ul class="posts">
	{%- for post in site.posts -%}
	<li>
		{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
		<div class="post-meta">
			<a class="post-link" href="{{ post.url | relative_url }}">
				<h2 class="post-title">{{ post.title | escape }}</h2>
			</a>
			<div class="post-date"><i class="icon-calendar"></i>{{ post.date | date: date_format }}</div>
		</div>
		<div class="post">
			{%- if site.show_excerpts -%}
			{{ post.excerpt }}
			{%- endif -%}
		</div>
	</li>
	{%- endfor -%}
</ul>
{%- endif -%}