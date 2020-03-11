+++
author = "digitaljoni"
categories = []
date = 2020-03-09T16:00:00Z
description = "Imagine you were given the task of creating an RPG set in the Dragonball universe and your task was to develop the Saiyan characters of the game. Here's a fun look at how to do OOP in Dart language."
image = "https://digitaljoni.com/images/oop-in-dart-dbz.png"
tags = ["presentation", "slides"]
title = "OOP in Dart - DBZ Edition"
type = "post"

+++
The following slideshow was part of my talk last February 2020 which gives a fun look at object-oriented programming in Dart. I used familiar anime characters to make it easy enough for beginners to understand and to be clear enough to illustrate objects in Dart language.

{{< slideshare id="GuVnMI18tDUKl7" >}}

Slide 1

Imagine you were given the task of creating an RPG set in the Dragonball universe and your task was to develop the Saiyan characters of the game. Saiyans are powerful beings from another planet that serves as the main characters of the series.

Slide 2

To make things simple, we represent a Saiyan object with two properties: the character's name and character's amount of power. And we give the character a few methods to punch, kick and do a special move. We also customize the toString() function to output the name and power.

Slide 3

Here we created 2 objects - "Goku" and "Vegeta" and test out their methods.

{{< dartpad id="5d4b8134eb09c2e6477e77a77f2e13b1" >}}

Slide 4

We then create a fight function to compare who has a higher amount of power. So in a fight with "Goku" and "Vegeta", "Goku" wins.

{{< dartpad id="afd3bb82ccab66df064c9b3c6633ca23" >}}

Slide 5

A new challenger approaches... "Broly" illustrates how we can define a named constructor to automatically define the amount of power the Saiyan object has. We used Saiyan.superForm() to create this new Saiyan object. Since it has a power greater than the two previous Saiyan objects, it will easily win in a fight individually.

{{< dartpad id="997ee71c457c1488517b03080be7bae0" >}}

Slide 6

In the Dragonball universe, Saiyans can do a fusion dance which results in them combining into one Saiyan with both their powers combined. Here we use this to illustrate Dart's feature of operator overriding. In this case, we override the plus (+) operator. So now if you add a Saiyan object with another Saiyan object, you will get a new Saiyan object with names and powers combined. Now if we use "Gogeta" and compare it to "Broly", the latter wins this round.

{{< dartpad id="1856b6fc5c62ce9cd99ede05b2e071c3" >}}

Slide 7

Just to keep things neat and proper, we move the "fight" function inside the Saiyan object.

{{< dartpad id="965b9e240a01326945424fb8244592e3" >}}

Slide 8

Later on into the Dragonball series, the Saiyans learn to enhance their power and become can now become "Super Saiyans". In this slide, we illustrate this by using Object Inheritance. The "SupaSaiyan" extends the "Saiyan" class and now you have a new object with a new property called "level" which basically represents the power level of the Saiyan object. If you have a power level of 2, it would result in double the power of the Saiyan.

{{< dartpad id="498ad0d40c8800970f8dbf2b89f12771" >}}

The Saiyan object examples illustrated here are far from perfect and can still be improved upon. Nevertheless, it is a start and you can use the concepts here for your projects.