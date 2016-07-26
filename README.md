# jill.js - jQuery Illustrator
---

jill.js is a Javascript interpretor that allows you to write code for HTML5 canvas elements in an object-oriented style.  Jill comes with some great classes for manilpulating colors, shapes, text, animations, interactions, and hopefully sounds.  All the fun of coding stuff withouth the hassle of having to creat the classes and interpretors. (Let me do that.) ;-)

---
## Changes
### 26 July 2016

In 2012, I attempted to make a project that would make creating HTML5 Canvas more object oriented.  Over the years new engines created by other users have come along.  They are more than likely better than jill.js, but I figure "what's one more thing to add to this market?"

Jill.js has been sitting on the backburner for some time now.  And considering I've been working on other HTML5 Canvas projects that won't render with my own code on Codepen.io, ether because I'm not self employeed or have a grant to fund some Silicon Valley Startup to sell their thing like they were Trump Steaks at The Sharper Image.

Considering I'm just some guy from the St. Louis area with a BSCS, I don't have that kind of money to promote how good my code is or the Venture Capital to *lie* to you saying how good my code is. :D

So here's the scoop:  Jill.js changes how you write JavaScript to process HTML5 Canvas.  I use functions and objects like classes like any reasonable JavaScript coder would do.  There are a few good resources for that that I'll gladly share in this README file to wrap your head around the concept of object oriented programming in a language that never really contained the structures for doing so.  There are ways around that, and to professionally sell yourself to the market, you should use them.

It is important to note that HTML5 Canvas does not have layers like SVG does.  Canvas elements are generally raster images (think MSPaint).  I have been having a fun time over the past few months playing with HTML5 Canvas interactively but I didn't integrate JQuery or Jill into that project.  And even though it was in straight JavaScript, it never processed on Codepen.io even after running it through JSHint and JSLint.  So one of my goals is to have Jill use `try...catch` blocks to throw errors that aren't difficult to understand and won't make you tear apart Jill components for something that happened in your code.

**"But what about `getContext`"?** Ah yes, `getContext`.  It does kinda suck that you want to use more than one `<canvas>` element, but then you have to do the whole `var c = document.getElementById("bob"); var ctx = c.getContext("2d");` thing and then having to make `ctx` an argument in whatever function you are doing because `ctx` is often declared globally.  I really want to fix that problem, and I hope that Jill can offer a solution so that you can code for multiple `<canvas>` elements and apply context functionality to as many canvas elements as you want.

One of the things I want to do is have Jill generate all this cool math stuff that looks like it would have been done in vector graphics.  Processing.js does something like this, but the way they write it is by making a JavaScript engine that understands the Processing Programming Language.  I don't want it to read from Processing.  If I had my way, I would have it read from C or C++ like from an OpenGL program.  Three.js does something similar to Processing but uses WebGL.  Which is great, and I highly recommend if you want to do something 3D related use Three.js.

Jill will still be in the realm of 2D for the moment and will proudly feature interactivity and animation like Processing.js only it won't be written like it was a program designed for Processing.js.  Long term goal would be to aim for some OpenGL syntax similar to how Three.js handles WebGL, but since I'm starting out small let's start with JavaScript first then try writing an interpretor that reads C/C++.

I had also made stuff that manipulates text and animation at one point and gladly want to revive that with what I've learned with the other project which didn't have a name really.

The return of the Jill.js part of a plan to renovate my website, JRCharney.com, over the next few months.  Hopefully when it's done you'll see some Jill.js stuff in action though I can't guarantee that it will look pretty in all browsers or on mobile devices.

Thank you for reading this document.
