---
layout: post
title: Drawing Circles - Math Meets Programming
---

I recently watched Moishe Lettvin talk ["What I Learned Doing 250 Interviews at Google"](https://www.youtube.com/watch?v=r8RxkpUvxK0). One of the points he brought is how diverse solutions can be for even simple problems. One question he was asked was to draw a circle. This is a great example of an onion question, one that has many layers of possible improvement.

The solution I would have come up with is a sampling of points using trigonometric functions. It ends up that this solution can be improved on substantially.

For instance, if I had thought a little bit more about the problem I could have potentially remembered the elegant solution `x^2 + y^2 = radius` and then fixing one variable `x = sqrt(radius - y^2)` and saved those computationally-expensive trigonometry functions.

Finally, there is [Bresenham's circle algorithm](https://en.wikipedia.org/wiki/Midpoint_circle_algorithm) which is apparently what DOS uses to draw circle. This is relatively complicated but draws all four quadrants of the circle at the same time.

<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/2/24/Bresenham_circle.svg" alt="Bresenham Circle Algorithm" />
</p>

This is one of the countless examples where having a deeper mathematical understanding leads to improved code.