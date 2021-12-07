---
layout: default
title: Initiatives
description: The intitiatives Shift SC puts on to promote human-centered and socially responsible tech at USC.
---

<section class="hero hero--single">

	<div class="hero__image" style="background-image: url({{ page.featured_image | relative_url }})">
		<div class="hero__overlay"></div>
	</div>

	<div class="wrap">

		<h1>Initiatives.md, an actual page yuh</h1>
		<p>This is how we do it babyyyy</p>

	</div>

</section>

<section class="listing">

	<div class="wrap">

		{% for project in site.initiatives reversed %}

		<article class="post">

			<div class="post__image-wrap">
				<div class="post__image" style="background-image: url({{ project.featured_image | relative_url }})"></div>
			</div>

			<div class="post__content-wrap">
				<div class="post__content">
					<h2 class="post__title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
					<p class="post__subtitle">{{ project.subtitle }}</p>
					<p class="post__description">{{ project.description }}</p>
				</div>
			</div>

		</article>

		{% endfor %}

	</div>

</section>