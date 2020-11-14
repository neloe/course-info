---
title: Using Netbeans
category: assign-info
layout: default
---

This semester we will be using Netbeans.
If you have not yet, follow the instructions in [Installing the JDK and Netbeans](devchain.html)

## Opening Projects

Once you have gotten a project (see [Getting and Submitting Assignments](assign_sub.html)), go to File->Open Project.
Navigate to where you downloaded the project.

![Open dialog]({{ "assets/img/nb/open_gradle.PNG" | relative_url }})

Notice the little elephant icon next to the project name; that indicates that this is the project you'll be opening.
If you don't see the elephant icon, you will need to switch directories.

## Running tests

Many of the labs and assignments are distributed with tests that will determine your "correctness" score.
You can run these tests to see how well your code works in projects that are distributed with these tests.
Note that this is different than running the `main` method.

In the Run menu, you should see an option titled "Test Project".  
Choosing that will run all tests associated with the project.
You can also hit Alt+F6.

![Run menu]({{ "assets/img/nb/runtests.PNG" | relative_url }})

You can also right click on a file in the left hand pane and select "Test File".
This will only run the tests for that one file.
You can also run the tests for the file you are currently working on with Ctrl+F6.

## Reading the output

The output will clearly show you the number of tests that pass or fail (notice the bottom pane) in the image above

![Test Output]({{ "assets/img/nb/output.PNG" | relative_url }})

You can expand tests that fail to get more information.

Double clicking on a failed test will bring you to a file in the Test Packages that will show you exactly what is being run to make the test fail.
Look at this testing code to figure out how your code might be failing and why it is not performing correctly!

![Failed Test]({{ "assets/img/nb/failedtest.PNG" | relative_url }})
