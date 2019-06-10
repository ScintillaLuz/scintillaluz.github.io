---
title: 'Content flow and layout for Bandcamp’s new home'
subtitle: ''
date: 2019-01-28 00:00:00
description: This page is a demo that shows everything you can do inside portfolio and blog posts.
featured_image: '/images/home-thumbs/homepage_thumb.jpg'
---

_**Filed under** UX/UI, Art Direction, Project Management, User Testing_


#### What were we doing, and why?

It was 2016, and our brand new editorial team was launching the _Daily_, *Bandcamp’s own independent music publication*. Mission of the magazine was to shed a light on the diverse world of Bandcamp’s artists, guiding fans through <a target="_blank" href="https://www.nytimes.com/2016/08/20/arts/music/bandcamp-shopping-for-music.html">“one of the greatest underground-culture bazaars of our time”</a>.

Up until the _Daily_ was born, the homepage represented Bandcamp’s main display window. *_With more than 600,000 artist sites, the homepage has been the compass of Bandcamp’s music discovery, tipping fans on where to look for the interesting stuff_*. Now that the _Daily_ was to lead in curating recommendations, it had to find its place on the homepage. Bandcamp’s home was due for a revamp.


#### What was I asked to do?

* Redesign the first half of our homepage, to fit a showcase of the _Daily_’s features.
* Design the flow for populating the homepage with editorial’s content.
* Design the internal dashboard to manage content’s upload for the homepage.


### Homepage Redesign

#### Old Home, New Plan

By the time I got assigned its redesign, Bandcamp’s homepage was divided in 7 sections, plus a fat footer. The first two thirds of the page were dedicated to _music discovery_, opening with a large full-width banner hosting the latest episode of our radio show, _The Bandcamp Weekly_. Following were a combination of smaller sections, offering different ways to browse, filter, and dig to find them music gems they’ve been looking for. Believing in user conversion through purchase, the CTAs for sign up were deprioritized, lining up at the very bottom of the page.

[GIFS old home]


#### Step One, Above The Fold

Before anything, I worked on the full-width banner to repurposed it. From the brief, it was to fit three or more _Daily_ headline, and the current Weekly episode. I started playing with big headlines on flat-coloured backgrounds, animated slideshows, and tiled grids. We called this module *_the carousel_*. My soft spot was for galleries with bright colours and full blown photographs, but considering mobile web performances we opted for a static carousel. The proposal that made the cut had no slideshow, with images arranged in a tiled layout. The mobile version used a nifty swiping pattern to scroll secondary headlines, maximizing the horizontal space with a catchy gesture.

<p style="font-size: 94%; color: #777777; margin-top: 30px;"><strong>Two proposals that we decided to archive</strong>. Good balance in the layout, but fat slideshows make for long loading times... often times boring users.</p>

[IMGs]


<p style="font-size: 94%; color: #777777; margin-top: 30px;"><strong>The final carousel</strong>. It’s not only a matter of performances. In this version, the layout’s hierarchy better supports the concept of highlighting an individual story. The main spot would host the most important feature of the day, with two of the smaller tiles dedicated to additional articles. A new episode of the Weekly would be featured every Tuesday morning PST, taking over the principal slot for the day.</p>

[IMGs]


#### Step Two, _Daily_  Recent News

The sales strip kept its current place, while we introduced the _Daily_ showcase right below it. Replacing two rows of album reviews and blog entry blurbs, this new section was intended to collect stories previously hosted in the _carousel_. Not all the content from the former layout was to be dismissed. Wrapped up in their own “New and Notable” section, the crispy three-sentences album review would be now owned and written by the editorial team.

On desktop I inherited a solid grid system, with overlaying 12 / 15 / 16 columns. I’ve designed both the _Daily_ news archive and the _New and Notable_ around a x15. The archive opener was a daily standard column called *Album Of the Day* – an original bit that was worth assigning a larger module to. Taking a cue from The Guardian’s homepage, I hid even more cards behind a toggle. The mobile version saw the _Album Of the Day_ expanding full width, presenting visitors a nice sequence of fresh content, before hitting older stories.

<p style="font-family: 'PT Sans', sans-serif; font-size: 98%; color: #888888; margin-top: 30px;"><strong>Structure brings on creativity</strong>. Playing with modules is pure design fun. Among several good candidates, we settled for the cleanest combination.</p>


#### Final Design

Check out this layout live on <a href="https://bandcamp.com">bandcamp.com</a>


> Presenting editorial content on the homepage was a visual design problem: grids, rhythm, whitespace balance. But solving how said content would dynamically flow into the page? That was UX design.


### Behind the Scenes

With the layout revamp came the request to work on a **custom content management solution for publishing editorial stories on the homepage**. Problems included:

* How content from the _Daily_ would be uploaded/selected/featured in the carousel.
* How editors would promote/demote a specific story in the main carousel spot.
* How/where the Weekly episode would be published on the carousel
* How Weekly and _Daily_ content in the carousel would interact.
* How carousel _Daily_ stories would move to the archival section below.
* How the Album of the Day would be updated, and where previous instances would show.

The three types of editorial stories — _Daily_ features, Weekly episodes, Album of the Day reviews — required different approaches. The Weekly was supposed to update automatically, as well as the Album of the Day. Editors wanted maximum flexibility for featuring and promoting content in the carousel – favouring a manual solution. Carousel older stories should then automatically be poured into the archival cards below.

I took these requirements and came up with a set of rules that combined automated and manual behaviors, designing a simple (proprietary) CMS system.




### Search Autocomplete (a two days hack)

Every year Bandcamp’s distributed team comes together to spend a week catching up, *in real life*. Usually working from our home offices, we get the chance to discover who’s actually very tall, and break the video chat habits. In 2017 me and Alexandra Hindley (Labels’ engineering lead) took over a 48-hours mini project, implementing a first version of an autocomplete in the homepage search bar.

<p style="font-size: 94%; color: #777777; margin-top: 30px;"><span style="color: #333333; font-weight: bold;">1.</span> Searching for a generic word. <span style="color: #333333; font-weight: bold;">2.</span> Searching for a keyword matching a music genre. The autocomplete returns a shortcut to the tag page, and a list of related tags/genres. – <span style="color: #333333;">
click on the images to enlarge</span></p>

<div class="gallery" data-columns="2">
	<img src="/images/homepage/autocomplete-01.gif">
	<img src="/images/homepage/autocomplete-02.gif">
</div>
