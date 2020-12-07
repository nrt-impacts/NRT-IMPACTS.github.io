---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: Homepage.png
widget1:
  title: "Upcoming"
  url: ''
  image: widget-1-302x182.jpg
  text: 'News<br/>
What is IMPACTS<br/>
Date: 2021<br/>
What is in the Program<br/>
More details here.'
widget2:
  title: "News & Events"
  url: ''
  text: '<em>November 30, 2020: Congratulations to Tammy Long and Robin Buell who were recognized at the NatSci Awards Ceremony on November 20<br/>
November 9, 2020: IMPACTS trainee Retreat on Nov 6 and 7<br/>
October 2, 2020: PLB 843 Forum in Computational Plant Science class going on in full swing during Fall 2020<br/>
September 7, 2020: Plants&Python course repository on GitHub preserved for 1000 years on film in the Github Arctic Code Vault<br/>
June 2, 2020:Rie Sadohara pursues internship in Summer 2020<br/> 
  .<br/>1. Language-Support :)<br/>2. Optimized for speed and it&#39;s responsive.<br/>3. Built on <a href="http://foundation.zurb.com/">Foundation Framework</a>.<br/>4. Seven different Headers.<br/>5. Customizable navigation, footer,...'
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
