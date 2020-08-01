---
layout: page
title: A Live Coding Experiment
---

Bret Victor's presentation [Inventing On Principle](http://vimeo.com/36579366) was thought-provoking. As a programmer, we have always known this but his emphasis on the point, that an immediate connection to creative output is enormously valuable, forces us to rethink about our tools and how we can improve them.

As I was watching his demo, I realized that the demo relied on certain assumptions. His prototype was for drawing an image on HTML5 canvas. One can easily imagine such a code editor for physical simulations as well. Both of these however are **passive** and **visual** in nature. An image is both static and passive, whereas a simulation is dynamic, but still passive. Both are visually perceived, so they can be grasped in an instant.

Most programs are not passive. Code is supposed to **do** things - manipulate the state of the universe. It's the correct **behaviour** that we are trying to achieve with our code. I started thinking about how we can immediately visualize the behaviour of code. Behaviour is such a transitive thing - it occupies time. Similar to audio (eg. music), visualizing the entire personality of code appears time-consuming. Code can't be summarized by data.

But can't it really? Almost immediately I realized that code itself can be used to capture the expected behaviour of another piece of code. By the means of **executable tests**. So the boolean test results are sufficient to explain whether a piece of code works correctly or not. It is possible to visualize the health of a codebase in an instant.

So I sat down and put together a minimal prototype for this.

<img src="/img/livecoding.png" width="100%" />

Of course, there are problems with live evaluation of code. One example is infinite loops which can be avoided by multiple threads. But seeing all the possible corner cases get resolved in real-time as you edit the code is incredibly fun. The bugs become immediately visible - making the programmer confident and happy. The longer it takes to realize that we made a mistake, the more miserable we feel. Nobody minds making a mistake when it can be immediately corrected. This also gives us an incentive to write comprehensive tests which is always a good thing.

I think this direction is worth exploring further. Full-fledged editors for general-purpose programming languages providing live testing capability would be a huge improvement to a programmer's workflow.

What do you think? [Let me know](http://twitter.com/nileshtrivedi).