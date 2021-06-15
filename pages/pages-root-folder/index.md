---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Widget No 1"
  url: 'The url to the widget'
  image: widget-1-302x182.jpg
  text: 'This is the description to the first widget. We meed to figure out whether we can have more than three widgets or if we are limited here.'
widget2:
  title: "Widget No 2"
  url: 'http://trust-cps-group.github.io/info/'
  text: 'The description of the second image. The link should actually lead somewhere. I have removed the video part which was present in the original page.'
widget3:
  title: "Widget No 3"
  url: 'https://github.com/trust-cps-group'
  image: widget-github-303x182.jpg
  text: 'The link should lead to the organization'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tinyletter.com/feeling-responsive
  text: Inform me about new updates and features ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
