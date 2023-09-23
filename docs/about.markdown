---
layout: page
title: About Us
permalink: /about/
---
<h2>Mission</h2>

<h3>Our Goal</h3>

<p>ZipCaptions aims to provide speech-to-text accessibility tools as widely as possible for as free as possible. We will work to find creative, responsible, effective solutions and make them available to as many people as possible.</p>

<p>We don’t want to build an app, we want to build a community of users, developers, and advocates to bring captions to as many creators across as many formats as possible.</p>

<h3>Our Model</h3>

<p>The popularity of recent developments in AI has brought with it opportunities to perform tasks such as speech recognition entirely within the browser. By performing the intense processing on the user’s computer as much as possible, we will keep our costs down, and accessibility up. This also has the added advantage of increasing privacy</p>

<h3>Our Method</h3>

<p>As many of our features as possible will be available for free to all users. We hope to grow a community of supporters - both financially and via pull requests to the codebase - to fund the operating costs. Where it’s not possible to provide free features, we may restrict access to supporters who fund the development and operation of ZipCaptions via Patreon.</p>

<h2>Values</h2>

<p>Our only value proposition is to provide a tool that makes adding accessibility to audio as freely available as possible. We have no investors, we have no shareholders - we are a pair of educators who want to empower people to set a standard of accessibility that has never before been possible.</p>

<p>We do not aim to make a profit - we aim to make a difference. </p>

<h2>Purpose</h2>

<p>There are environments in which accessibility was previously out of reach - classroom, in-person meetings, board rooms, large gatherings - and we want to change that. Other tools often require paid subscriptions, feature obnoxious advertisements, or sell your personal data, our purpose is to offer an alternative that is free and open.</p>

<h2>Vision</h2>

<p>We believe that people will support a tool that provides them value, and will empower us to bring accessibility to as many people as possible. We will be supported by, and we will be working for, our community, to build something that will help make a difference.</p>

<h2>Responsibilites</h2>

<p>ZipCaptions is currently operated on an entirely voluntary basis by two educators based out of Quebec, Canada. Chris is responsible for operations - general management, finances, communications, marketing, support, and content. James is responsible for the technical aspects - development, hosting, integrations, bugs, etc. The feature roadmap is built in collaboration with our community of supporters on Patreon.</p>

{% for staff_member in site.staff_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
