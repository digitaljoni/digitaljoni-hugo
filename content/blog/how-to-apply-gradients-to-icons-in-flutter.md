+++
author = "digitaljoni"
categories = []
date = 2020-03-17T14:00:00Z
description = ""
draft = true
image = ""
tags = []
title = "How to Apply Gradients To Icons in Flutter"
type = "post"

+++
There will be times that a colored icon won't be enough for the UI that you are building in Flutter. How about if we put a gradient color on the icon instead? 

The problem is that there is no gradient method on the Icon widget. So we need to use a ShaderMask widget and wrap around the Icon. Here's an example implementation and called it GradientIconWidget:

{{< gist digitaljoni 1ad947b17f1898f19db74546485674e0 >}}

In order to use this, all you need to do is to pass the icon and gradient that you would like to apply:

{{< gist digitaljoni 354e35fe2f249ba23d58a2720cc69cc1 >}}

I hope this helps you on your next project!