---
layout: default
title: Your New Jekyll Site
---

<div id="articles">
  <h1>Articles</h1>
  <ul class="posts noList">
    {% for post in site.posts %}
      <li>
      	<span class="date">{{ post.date | date_to_string }}</span>
      	<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      	<p class="description">{% if post.description %}{{ post.description  | strip_html | strip_newlines | truncate: 120 }}{% else %}{{ post.content | strip_html | strip_newlines | truncate: 120 }}{% endif %}</p>
      </li>
      <div class="about-content">		
					<h2>Belajar bersama Upin & Ipin</h3>			
					<h3>Doa Niat Berpuasa by Upin & Ipin</h3>
					<p>Silahkan klik Play.</p>
						<audio controls="controls" widht="100%" height="auto">
							<source src="/Iwan_Fals_Kemesraan.ogg" />
							Teks ini akan muncul jika browser tidak support HTML5 Audio tag.
						</audio>
					</br>
					<h3>Doa Berbuka Puasa by Upin & Ipin</h3>
					<p>Silahkan klik Play.</p>
							<audio controls="controls" widht="100%" height="auto">
								<source src="/Nike Ardilla - Bintang kehidupan.ogg" />
								Teks ini akan muncul jika browser tidak support HTML5 Audio tag.
							</audio>
						
				</br></br></br>
		</div>
    {% endfor %}
  </ul>
</div>
