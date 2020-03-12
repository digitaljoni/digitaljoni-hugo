+++
categories = []
featured_image = ""
image = "https://digitaljoni.com/images/project_noizart.jpg"
showcomments = false
showmeta = false
slug = "noizart"
tags = []
title = "NoizArt Project"
type = "page"

+++
The NoizArt project started as an inspiration from Robert Felker (aka The Flutter Artist) where he creates artwork using Dart and Flutter. 

In this project it would be a bit different though. Basically most decisions on how the artwork is rendereed are left to the program itself. 

It uses the built-in function "random" to make the decisions it uses a "seed" value of the current timestamp. Based on the results, the program goes through a decision tree to determine various aspects of the art: canvas color, color theme, what to draw, will there be a foreground, midground and background, and more!

I am currently constructing and tweaking the decision tree and adding more things that can be rendered. It's kinda like teaching the program how to draw or paint.

In the future, I may also hook this up in an external source, i.e. a weather api to give it sort of a "mood" to sway its decision making process. It may affect what type of colors it will choose if the weather is gloomy or happy... and it may not draw anything at all.

What comes out of this is a unique artwork as a result.