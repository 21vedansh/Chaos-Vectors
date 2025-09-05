# Chaos Vectors
This project is just me messing around with **HTML5 Canvas** to see what kind of trippy patterns I could come up with.
It turned into a whole "flow field", basically a bunch of tiny vectors dancing all around based on some mathy rules.

## What's going on here?
At its heart, the thing is quite simple
1. Imagine the screen as a giant grid, divided into small cells.
2. At each point in the grid, calculate a direction (an angle) using some formula.
   - rn, I'm using **sin+cosine** function mixed with some mouse position to make it reactive.
   - This gives each particle a direction, like little arrows in a magnetic field.
3. Draw tiny lines that follow those directions.
4. Keep updating every frame with `requestAnimationFrame`, so the field comes alive.
That's it, add some colors, gradients, chaos, and you get something that looks alive. 
