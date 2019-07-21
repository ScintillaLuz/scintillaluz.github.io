---
title: 'Building a scalable post purchase experience'
subtitle: ''
date: 2019-06-01 00:00:00
description: Redesigning the post purchase experience for mobile web, fan app, and desktop
featured_image: '/images/home-thumbs/post_purchase_thumb.jpg'
---
_**Filed under** UX/UI (Desktop, Mobile, App), User Testing_



#### What were we doing, and why?

At the end of 2015 I was busy introducing credit card payments. Up until then the only payment system available was PayPal. Restructuring the purchase flow, I took a stab at improving the page where buyers would land after they complete their purchase.

**The post purchase page**—**PPP, informally**—was not designed around a grid, and wasn’t visually consistent across platforms. I discussed the opportunity to make the PPP redesign its own project with the design manager. He supported the decision telling me “this is Bandcamp’s most important page.” “No pressure!” could have been a timely response, but I do love a design challenge.

#### What was I asked to do?

* Redesign the post purchase experience for mobile web, desktop, and the fan app.
* Create layout and logic that would make the post purchase page **scalable in two ways**:
  * In itself, going from single item purchases to large shopping carts with a complex mix of items.
  * For when new types of items would be available for purchase (ex: gift cards.)
* **Focus the communication on streaming**, nudging users to install our listening app.



## Preliminary Work

Before design, there’s research. First steps were:
1. Establishing user needs, to define the scope of the redesign.
2. Defining what a successful design would do, for business needs.
3. Analyzing the current PPPs, and their shortcomings.

<div class="gallery" data-columns="1" style="max-width: 860px;">
	<img src="/images/ppp/01-user-needs.jpg">
</div>

After clarifying what the page *should do*, I took screenshots of the current PPPs, and built an inventory of all the cases. I took notes on why the PPP wasn’t supporting user needs correctly—structurally and visually.



## Designing for Scalability

The number of PPP cases and their characteristics depends also on the nature of the items sold. Before diving into UX details, I wanted to answer the question: ***what are all the items artists can sell on Bandcamp?***

<div class="gallery" data-columns="1" style="max-width: 860px;">
	<img src="/images/ppp/02-type-of-items-sold.jpg">
</div>

With this in mind, and the cases inventory at hands, I started working on the ***information architecture***.

Only a very small percentage of purchases belonged to carts, I started with single item purchases, and made them the baseline. The idea was to discover recurring patterns among cases, and turn them into logical/visual modules in the new design.

<p style="font-size: 94%; color: #777777; margin-top: 35px; font-style: italic;"><span style="color: #333333;"><strong>Information architecture, single purchase cases tree. </strong></span> Left column: the common patterns I identified; right: ramifications of the cases. The animation highlights the patterns’ distribution among the cases.</p>

<div class="gallery" data-columns="1" style="max-width: 1200px;">
	<img src="/images/ppp/03-information-architecture-GIF.gif">
</div>



## The Solution: Function & Layout

### The Context

The purchase experience was shaped by a number of attributes:

* *Purchase mode*: single vs cart
* *User status*: logged in fan / logged out fan (recognized by email) / non-fan (user without an account)
* *Item category*: digital vs merch
* *Item type*: standalone digital / package digital / gift / ... (as seen in the above diagram)
* *Platform/Device*: web & mobile web, iOS vs Android apps

Also important to consider:

* **Bandcamp allowed guest checkouts**, but we still wanted to encourage account sign up on the PPP.
* **Users were mostly buying from a personal computer.**
* Permutations on the PPP added up to about 150, but **carts were a minority case.**

Seeing the last point, I started to **design the single purchase layout**, and work later on carts as its extension. I set off re-arranging elements on the page to a **clearer hierarchy**, and changing proportions accordingly. I made the streaming promo and purchase thumbnail the focus of the new layout.



### Single Purchase Layout

The final design was organized differently on different platforms, but all layouts followed the idea of a hierarchical page, and shared the same visual language. Later, by management’s request, the desktop re-design would change focus and promote streaming in the app, while downplaying file downloads.

Design for the single purchase of a logged-in fan would become the foundation of all the following cases.

![](/images/ppp/04-single-purchase-final-layout.jpg)


#### Signed up user (“Fan”) — Old vs New

<p style="font-size: 94%; color: #777777; margin-top: 20px; font-style: italic;">It is interesting to notice how the old page was so visually unbalanced. Header and footer took over most of the space, surrounded by flat typography that did not take into account hierarchies.</p>

<div class="gallery" data-columns="2">
  <img src="/images/ppp/05-single-desktop-old.jpg">
  <img src="/images/ppp/06-single-desktop-new.jpg">
  <img src="/images/ppp/07-single-mobile-old.jpg">
  <img src="/images/ppp/08-single-mobile-new.jpg">
  <img src="/images/ppp/09-desktop-skeleton-GIF.gif">
  <img src="/images/ppp/10-mobile-skeleton-GIF.gif">
</div>



#### User with no account (“Non-fan”) — Old vs New

<p style="font-size: 94%; color: #777777; margin-top: 20px; font-style: italic;">There is a fundamental shift in this version. Where the previous page includes the promo as an extra element added at the bottom of the page, the newer layout makes the sign up CTA the core message of the page.</p>

<div class="gallery" data-columns="2">
  <img src="/images/ppp/11-single-desktop-nf-old.jpg">
  <img src="/images/ppp/12-single-desktop-nf-new.jpg">
  <img src="/images/ppp/13-single-mobile-nf-old.jpg">
  <img src="/images/ppp/14-single-mobile-nf-new.jpg">
  <img src="/images/ppp/15-desktop-nf-skeleton-GIF.gif">
  <img src="/images/ppp/16-mobile-nf-skeleton-GIF.gif">
</div>



#### Other Single Purchase Cases

In the old layout, a graphic element was sometimes added to the thumbnail: a pre-order banner or a ribbon for gifts, for example. Cover artworks and merch thumbs had different proportions: the obvious square for covers, and 4:3 for physical items. In my re-design **I methodically organized thumbs and their graphic add-ons into a visual system, ending up with 12 thumb variations**.

<div class="gallery" data-columns="2">
  <img src="/images/ppp/17-thumbs-variations.jpg">
  <img src="/images/ppp/18-thumbs-layout-variations-GIF.gif">
</div>



<p style="font-size: 94%; color: #777777; margin-top: 35px; font-style: italic;"><span style="color: #333333;"><strong>More single purchase cases.</strong></span> Between desktop and mobile web, there were about 30 x 2 (60) cases.</p>

<div class="gallery" data-columns="2">
  <img src="/images/ppp/19-digital-pre-order.jpg">
  <img src="/images/ppp/20-mobile-digital-pre-order.jpg">
  <img src="/images/ppp/21-merch-w-digital.jpg">
  <img src="/images/ppp/22-mobile-merch-w-digital.jpg">
  <img src="/images/ppp/23-merch-w-digital-pre-order.jpg">
  <img src="/images/ppp/24-mobile-merch-w-digital-pre-order.jpg">
  <img src="/images/ppp/25-merch-w-digital-nf.jpg">
  <img src="/images/ppp/26-mobile-merch-w-digital-nf.jpg">
</div>


#### Download Options

A download is just a... download, right? Actually, downloading is not necessarily straightforward:
1. On *desktop*, users would get to pick a format before getting their tracks in a .zip
2. On *mobile web*, downloading was either not allowed (iOS), or confusing even for tech savy users (Android)

**Desktop solution:**
* On their first purchase, users would get a generic “download” button
* Format options would be grouped based on fidelity
* After choosing, the format preference was saved for the next purchase

![](/images/ppp/27-desktop-download-GIF.gif)

**Mobile web solutions:**
* With phones not reliably supporting downloads, the fastest way to listen was creating an account
* The alternative was downloading on a computer, and then transferring to the phone. With this in mind:
  * I re-wrote instructions on transferring files to a phone (iOS vs Android)
  * I corrected Android instruction for users who wanted to try downloading anyway


![](/images/ppp/28-android-download-GIF.gif)


#### Single purchase, but multiple downloads

The last case was the *Full Discography*, a package including multiple downloads. Visually, this layout took me a step closer to solving carts, with a solution for a purchase including more than one digital item and the corresponding downloads. In fact, a discography was offered as a series of releases, which would have to be downloaded separately.

<div class="gallery" data-columns="1" style="max-width: 760px;">
  <img src="/images/ppp/29-desktop-full-discography-GIF.gif">
</div>



### Multiple Purchases: Carts

**To make sense of carts, I went back thinking on the item’s type**. Instead of grouping items by digital vs physical vs digital+physical, I defined similarities by looking at what was the primary need. What did I know that could help me categorize the different items in a cart?
* Digital items would all be available for streaming. The message was the same.
* Digital items would come with a download (taking me back to the discography’s layout).
* Merch items had an estimated delivery time, and possibly options for size/color/quantity.
* On the buyer’s side, gifts never had a download, but would mention the email and physical address of the giftee.

With this in mind I ended up with a **page with three sections**:
1. **Digital releases**: similar to a discography, with a button toggling the full list of downloads.
2. **Physical orders**: listing only ETAs and other meaningful info.
3. **Gifts**: both digital and physical.

In the final cart design, ***all the possible cart combinations would generate only 6 layouts***.

![](/images/ppp/30-carts-layout-taxonomy.jpg)


<p style="font-size: 94%; color: #777777; margin-top: 35px; font-style: italic;"><span style="color: #333333;"><strong>Cart purchase with digital, merch, and gifts.</strong></span> Physical orders and gifts are essentially the same on both platform. The real difference is with the digital component.</p>


<div class="gallery" data-columns="2">
  <img src="/images/ppp/31-cart-digital-merch-gifts.jpg">
  <img src="/images/ppp/32-cart-pre-orders-disco-gift.jpg">
</div>



## Conclusions

* After the launch we recorderd a significant increase in app installs
* As of today, the PPP remains the first place fans get to know about our apps
* Later we introduced two other types of items for purchase, without changing anything in this design
* On the other hand… **desktop users wanted to see the download first**. The streaming message was important communication for us, but not a priority for fans. The plan is to go back and reexamine the issue, honoring real users’ needs first.
