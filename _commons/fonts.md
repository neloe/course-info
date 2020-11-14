---
title: Fonts
layout: default
category: general
---

Let's briefly talk about fonts in an IDE.

If you think about reading a book or a web page, there is a lot of research about how readable a font is and the effects of kerning (letter spacing), ligatures, serifs, and other elements to improve comprehension.
The funny thing about reading is that the human mind is pretty good at covering for information and filling in the blacnks enabling us to read and comprehend more quickly.
The role of an individual character is less important.

In programming, though, every character makes a difference.
A single typo, or an added space can render a program uncompilable, or at the very least introduce logical bugs that give incorrect answers.
In prose, this might slow down a reader, but not make text incomprehensible.

As such, fonts that make for good reading of literature don't necessarily make for good fonts in an IDE.
Some think that the answer is "Just use a monospace font!", but that may not be enough.
We use monospace fonts to make alignment of source code easier (varying width spaces are HORRIBLE).
Consider the following text (image, because embedding fonts in markdown is hard):

![Courier New]({{ 'assets/img/fonts/courierl1.PNG' | relative_url }})

Can you tell the difference between a 1 and an l?  
You may be able to, but it may take a few seconds.  
This example is directly based on experiences I've had with students in this course in the past (naming a variable a lower case L can really mess with people's heads).

What about the following text:

![Calibri]({{'assets/img/fonts/calibriIl.PNG' | relative_url}})

Which are lower case L's, and which are upper case i's?

A good programmer's font will allow you to easily distinguish between different similar characters.

Consider the above texts, but in a different font:

![Hack l1]({{'assets/img/fonts/hackl1.PNG' | relative_url}})

![Hack lI]({{'assets/img/fonts/hacklI.PNG' | relative_url}})

The first two examples use Courier New (a variant of the Courier font, which is available almost universally and frequently the default for consoles and IDEs) and Calibri (the default "paragraph" font in MSWord).
The font used for examples 3 and 4 are from a font called Hack (a typeface designed for programmers).

Choice of font is ultimately up to personal preference.  
However, choosing a font designed for programming makes coding a much more pleasant experience.
The default font in IntelliJ IDEA depends on your system (I have never found a system where I loved the default, though on my Linux computer it defaulted to DejaVu Sans Mono, which isn't the worst font in the world).
There's a chance on your computer it will default to Courier New.
I highly recommend you take some time and experiment with some fonts.
Not only can they make reading your code easier, but they can also make the activity feel less archaic (Courier is *so* 80s).

Personally, I quite like the [Hack font](https://sourcefoundry.org/hack/); to me it is easy to read and comprehend.
It's also the first font that I found that I liked, so I can honestly say that I haven't looked actively for several years.
Other developers quite like [Inconsolata](https://fonts.google.com/specimen/Inconsolata),
Others have found other fonts they enjoy (Droid Sans Mono, etc).
A quick Google search brought me to [this page](http://hivelogic.com/articles/top-10-programming-fonts/), and other searches will bring you different results.

It may seem like a small and trivial change to make, but in my experience I have found that choosing a font I find pleasing makes programming an easier and more streamlined task.
One of the first things I do on ANY new computer I work on (that I'm allowed to) is install the Hack font, then change my editors and console windows to use the font.
I *highly* recommend you take the time to find a font you like.
Even small changes like this can add up to a much more pleasant experience, and the less time you spend thinking about what individual characters are, the more time you can spend actually solving the problems you are writing code for.
