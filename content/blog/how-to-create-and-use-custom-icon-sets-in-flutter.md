+++
author = ""
categories = []
date = 2020-03-08T16:00:00Z
description = ""
image = ""
tags = []
title = "How to Create and Use Custom Icon Sets in Flutter"
type = "post"

+++
Flutter comes with a big library of built-in icons that you can use on your projects. In most projects, these icons should be enough, however, if you need to use custom icons, you will need to create your own icon font. 

Here’s a quick guide on how to create an icon font for your Flutter app:

1. You would need to create SVG vectors for your icon images. You can use Adobe Illustrator or Sketch to create vector files. These vectors need to be wellmade - meaning it has to be a flat shape with no extra layers or masks.
2. Then export the vectors into individual SVG files.
3. Next, you need to go to FlutterIcon.com and drag and drop the files to the page. This will upload your SVG files and then convert them into icons.
4. You can select and deselect the icons you would like to export by clicking on them. You can even edit details of the icon by tapping the edit icon.
5. Once you are done, enter a name then, click on the Download button to download the icon set.
6. This will package your vector icons and produce a zip file with the following files:

* TTF font file - vector icons converted and packaged into a single TTF font file
* Dart file - the .dart file that you can import to your app
* Config.json - you can use this to add more icons later

Using the Custom Font

1. Drag and drop the TTF file and to the assets folder
2. Drag and drop the dart file to the lib folder
3. Open main.dart and import the dart file
4. On a widget, add a child and use Icon widget