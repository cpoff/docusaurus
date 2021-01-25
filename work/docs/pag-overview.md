---
title: PAG Overview
sidebar_label: Overview
slug: pag-overview
---


PAG has a dynamic construction, build using a few modules and frameworks not used on RTA. It allows a more automated flow of content to their respective sections.

### Category pages

Category index pages are mostly built using the WP Show Posts plug-in. It allows the admin to select the display characteristics, and content assignments. For example: The WP Show Post entry for the Mobility category page would be: show headline, summary (75 words), drawing Posts or Pages from the Mobility category You can also assign specific or multiple tags instead of category.


### Homepage
This uses the [Unsemantic CSS framework](https://unsemantic.com/) for the table. Unsemantic is compatible with the Generate Press theme, so it uses common div tags and responds well to mobile devices. It's a grid layout similar to Bootstrap and based on points from a 1-100 scale. So in the example below, something might have ...

```html
lgc_column grid="30" tablet_grid="45" mobile_grid="100"
```
Meaning that element is 100% width on mobile device, 45% on table, and 30% on desktop.

You can also place those attributes directly into div tags:

```html
<div class="grid-container">
  <div class="grid-25">
    I am 25% wide.
  </div>
  <div class="grid-50">
    I am 50% wide.
  </div>
  <div class="grid-25">
    I am 25% wide.
  </div>
</div>
```

Example full page code:

```html
[lgc_column grid="10" tablet_grid="5" mobile_grid="5" last="false"][/lgc_column]

[lgc_column grid="30" tablet_grid="45" mobile_grid="100" last="false" class="col1" equal_heights="true"]

<img class="img1" src="/wp-content/uploads/sites/6/2020/08/MapsDataIcon.png" /><a href="/info-center/maps-and-data/"><b>Maps and Data</b></a>
Explore a variety of map viewer tools to learn about our region.

<img class="img1" src="/wp-content/uploads/sites/6/2020/08/BikePedIcon.png" /><a href="/mobility/bicycle-and-pedestrian-safety/"><b>Bike &amp; Pedestrian Safety</b></a>
Safety is a regional goal. Learn about bicycle and pedestrian safety tips.

<img class="img1" src="/wp-content/uploads/sites/6/2020/08/2045Icon.png" /><a href="/mobility/regional-mobility-and-accessibility-plan/"><b>Regional Mobility &amp; Accessibility Plan</b></a>
Take a look at our 25-year regional transportation plan.

[/lgc_column]

[lgc_column grid="30" tablet_grid="45" mobile_grid="100" last="false" class="col1" equal_heights="true"]

<img class="img1" src="/wp-content/uploads/sites/6/2020/08/TravelDataIcon.png" /><a href="https://pag.ms2soft.com/tcds/tsearch.asp?loc=Pag&amp;mod=" target="_blank" rel="noopener noreferrer"><b>Travel Data</b></a>
Curious about traffic patterns? View regional traffic counts.

<img class="img1" src="/wp-content/uploads/sites/6/2020/09/PubParticipationIcon.png" /><a href="/get-involved/public-participation/"><b>Public Participation</b></a>
Learn how you can participate in the planning process.

<img class="img1" src="/wp-content/uploads/sites/6/2020/08/TIPIcon.png" /><a href="/mobility/transportation-improvement-program/"><b>Transportation Improvement Program</b></a>
Find out what transportation projects are in the pipeline.

[/lgc_column]

[lgc_column grid="20" tablet_grid="100" mobile_grid="98" last="false" equal_heights="true" class="boxNew"]
<div class="testyHome">
<h2>Regional Connections</h2>
<h4 style="margin-top:-20px;">December 2020</h4>
<img src="/wp-content/uploads/sites/6/2020/10/RCpeople.jpg" />
<a class="button" href="/tag/regional-connections-dec-2020/">Learn More</a>
</div>
[/lgc_column]

[lgc_column grid="10" tablet_grid="5" mobile_grid="5" last="true"][/lgc_column]

<div class="newsyHome">
<h2>News Summary</h2>
[wp_show_posts id="2358"]
<a class="button" href="/info-center/news/">More News</a>
</div>
```
