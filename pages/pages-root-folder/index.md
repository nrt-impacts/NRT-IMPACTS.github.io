---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image: "grapevine_leaf-970x.jpg"
  background-color: "#fabb00"
widget1:
  title: "Upcoming"
  url: ''
  image: widget-1-302x182.jpg
  text: 'Corteva-PBGB-NRT Symposium<br/>
Phenomic Applications in Plant Breeding<br/>
Date: December 12-13th, 2019<br/>
Registration Deadline: Wednesday, November 27, 2019<br/>
General Registration link<br/>
Poster Registration link<br/>
Mini Data Carpentry Genomics Workshop schedule<br/>
More details here.'
widget2:
  title: "News & Events"
  url: 'http://phlow.github.io/feeling-responsive/info/'
  text: '<em>Feeling Responsive</em> is heavily customizable.<br/>1. Language-Support :)<br/>2. Optimized for speed and it&#39;s responsive.<br/>3. Built on <a href="http://foundation.zurb.com/">Foundation Framework</a>.<br/>4. Seven different Headers.<br/>5. Customizable navigation, footer,...'
  video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Twitter"
  url: 'https://twitter.com/nrt_impacts?ref_src=twsrc%5Etfw%7Ctwcamp%5Eembeddedtimeline%7Ctwterm%5Eprofile%3Anrt_impacts&ref_url=https%3A%2F%2Fimpacts.natsci.msu.edu%2F'
  image: twitter.svg
  text: 'via Twitter <a href="http://twitter.com/nrt_impacts">@nrt_impacts</a>.'
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
