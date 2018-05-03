---
layout: page
title: About
description: Some description.
permalink: /photos/
---
<style>
  @import url(https://fonts.googleapis.com/css?family=Open+Sans);


#instafeed {
  width: 100%;
  display: flex;
}
#instafeed a {
  position: relative;
  width: 50%;
}
@media only screen and (min-width: 580px) {
  #instafeed a {
    width: 25%;
  }
}
#instafeed a img {
  display: block;
  width: 100%;
  height: 100%;
}
#instafeed a div.footer {
  width: auto;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: .5rem 1rem;
  background: rgba(30, 144, 255, 0.8);
  font-size: .8rem;
  font-family: 'Open Sans', sans-serif;
  color: white;
  text-transform: uppercase;
}
#instafeed a div.footer img {
  height: 40px;
  width: 40px;
  border-radius: 50%;
  margin-right: .5rem;
  box-shadow: 0 0 0 1px rgba(255, 255, 255, 0.4);
}
#instafeed a div.user {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
#instafeed a div.caption {
  height: 0;
  opacity: 0;
  margin-bottom: 0;
  background: rgba(0, 0, 0, 0.2);
}
#instafeed a:hover .caption, #instafeed a:focus .caption {
  margin: -.5rem -1rem .5rem;
  padding: .5rem 1rem;
  opacity: 1;
  height: auto;
}

  </style>

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

{% include insta.html id=page.instagram %}
