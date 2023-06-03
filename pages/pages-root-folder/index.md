---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage

title: "Multipixels"

# about:
#  text: "Lorem ipsum dolor sit amet. Eum eaque odit aut eaque necessitatibus et soluta fugit. Aut dicta voluptatem sit error excepturi ut temporibus optio qui nobis consequatur nam ratione ratione est voluptatum cupiditate et labore adipisci. Eum velit suscipit eum dolorem voluptatibus ut cumque recusandae sed sunt quasi non eligendi distinctio. In ipsa consequatur et unde fuga et architecto quia. 
#  <br><br> 
#  Sit atque consequuntur est accusantium iusto non itaque dolorem et facere quas quo harum veniam ut galisum debitis. Ex temporibus sapiente ut quisquam repellendus ut nihil eaque ea dolorum officia non vitae delectus! Eum totam nemo vel facere obcaecati non ullam eveniet ab ullam numquam 33 enim sunt et fuga impedit et suscipit pariatur. Ea internos aliquid 33 tempora veritatis et autem fuga ex aliquam voluptatibus in quasi sapiente qui deleniti assumenda in distinctio ullam."

widget1:
  title: "KTaNE Assistant"
  url: '/projects/ktane-assistant'
  text: 'A high-school project made to help users play Keep Talking and Nobody Explodes without the need of another player. Simply start up the program and describe the bomb as it tells you which wires to cut or what code to insert.'
  video: '<a href="#" data-reveal-id="videoModal"><img src="images/widget1-thumb.png" width="100%" alt=""/></a>'
widget2:
  title: "Crop Rush"
  url: '/projects/crop-rush'
  image: projects/crop-rush-thumb.png
  text: "A game made for the Ludum Dare 52 game jam. Crop Rush is a short puzzle game in which the player has to harvest all the crops in the least amount of moves possible. The game is inspired by Club Penguin's Thin Ice minigame"
widget3:
  title: "Nyctomorph"
  url: '/projects/nyctomorph'
  image: projects/nyctomorph-thumb.png
  text: "A game made for the 5th NOKIA 3310 Game Jam game jam. Nyctomorph is a short survival adventure game in which the player has to survive the night, alone in a dark forest, with only a campfire and a handful of twigs scattered about. Don't stray far from the light... who knows what could be lurking about?"

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
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html

#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

# About Me

Lorem ipsum dolor sit amet. Eum eaque odit aut eaque necessitatibus et soluta fugit. Aut dicta voluptatem sit error excepturi ut temporibus optio qui nobis consequatur nam ratione ratione est voluptatum cupiditate et labore adipisci. Eum velit suscipit eum dolorem voluptatibus ut cumque recusandae sed sunt quasi non eligendi distinctio. In ipsa consequatur et unde fuga et architecto quia. 

Sit atque consequuntur est accusantium iusto non itaque dolorem et facere quas quo harum veniam ut galisum debitis. Ex temporibus sapiente ut quisquam repellendus ut nihil eaque ea dolorum officia non vitae delectus! Eum totam nemo vel facere obcaecati non ullam eveniet ab ullam numquam 33 enim sunt et fuga impedit et suscipit pariatur. Ea internos aliquid 33 tempora veritatis et autem fuga ex aliquam voluptatibus in quasi sapiente qui deleniti assumenda in distinctio ullam.

<div id="videoModal" class="reveal-modal" data-reveal aria-hidden="true" role="dialog">
  <h2> KTaNE Assistant Video Demo </h2>
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/qaytGFiAcFE" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
  <a class="button tiny radius" href="{{ widget_1.url }}">Project Page ></a>
</div>
