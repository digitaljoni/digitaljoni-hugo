+++
author = "digitaljoni"
categories = ["git"]
date = 2020-03-13T16:00:00Z
description = "There will be times when you have a file that you would need to edit to test something in your app and you do not want to commit those changes to the repository. "
image = "https://digitaljoni.com/images/workflow_blog.jpg"
tags = ["tips"]
title = "Git tips: How to Ignore changes to a tracked file"
type = "post"

+++
There will be times when you have a file that you would need to edit to test something in your app and you don't want to commit those changes to the repository. Let’s say you have config_dev.dart currently containing settings of your app in a development environment:

    const String apiUrl = “localhost:3000/api/articles/“
    const bool debugMode = false;

Now, for example, you would need to change the URL of the API to point to another local machine or test server within your network. This is how it would look like:

    const String apiUrl = “http://192.168.1.200:3000/api/articles/“
    const bool debugMode = true;

If you save this file, git will tell you that there are changes to the file. Since these changes are only temporary, it would be annoying to revert it back once you are done testing. And if you keep on changing this file in the future, you would need to repeat the process over and over again.

Instead, you can use the following command to **disable change tracking on the file**:

    git update-index —assume-unchanged lib/config_dev.dart

So now you can change config_dev.dart as much as you want and any changes are ignored by Git.

If you want Git to **resume tracking any changes to the file**:

    git update-index —no-assume-unchanged lib/config_dev.dart

I hope this helps you! It sure was a time saver for me!

Please note, this is not the same as using .gitignore. If you add a file to the .gitignore file, Git will delete the file entirely from the repository on the next **git commit** and we don’t want to do that for important files.