---
layout: page
title: Hello.
# tagline: Supporting tagline
---
{% include JB/setup %}

I'm a lifelong computer geek, California native, indie music enthusiast and sports fan residing in San Francisco.

Professional interests: highly scalable and available architectures; agile and lean product development; building a great, fun and accountable team culture

Teams: [California Golden Bears](http://californiagoldenblogs.com), Arsenal Gooners, San Francisco Giants

Music: I'm a dad now, so it is increasingly hard to listen to anything but the Toddler Radio channel. Past favorite festivals: [Portland's Musicfest NW](http://musicfestnw.com/), [Brooklyn's Northside](http://northsidefestival.com/)

Other interests: travel, [dive bars](http://www.yelp.com/biz/lucky-13-san-francisco), [street food](http://www.ladyironchef.com/tag/best-hawker-centre-singapore/)

<div>
    
  {% for post in site.posts %}
    <hr>
    <div>
        <div class="span5">
	        <h4><strong><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></strong></h4>
            <p>
                {{post.summary}}
            </p>
            <span>{{ post.date | date_to_string }}</span>
            <p><a href="{{ post.url }}">Read more</a></p>
        </div>
    </div>
  {% endfor %}
</div>

