---
layout: page
title: About
description: Some description.
permalink: /photos/
---

<img itemprop="image" class="img-rounded" src="https://res.cloudinary.com/dm7h7e8xj/image/upload/c_fill,h_200,w_200/v1504971955/neo_ruqszk.jpg" alt="Your Name">

## photos

<div id="instafeed">
</div>
<!-- Use the CDN or host the script yourself -->
<!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/instafeed.js/1.4.1/instafeed.min.js"></script> -->
<script src="https://matthewelsom.com/assets/js/libs/instafeed.min.js"></script>
<script type="text/javascript">
  var userFeed = new Instafeed({
    get: 'user',
    userId: '623597756',
    clientId: '02b47e1b98ce4f04adc271ffbd26611d',
    accessToken: '623597756.02b47e1.3dbf3cb6dc3f4dccbc5b1b5ae8c74a72',
    resolution: 'standard_resolution',
    template: '<a href="{{link}}" target="_blank" id="{{id}}"><img src="{{image}}"/><div class="footer"><div class="caption">{{caption}}</div><div class="user"><img src="{{model.user.profile_picture}}"/><span>{{model.user.username}}</span></div></div></a>',
    sortBy: 'most-recent',
    limit: 2,
    links: false
  });
  userFeed.run();
</script>
