# Matrix Range

A shooting-range trainer for the 2D model transformations chapter of CS 451 (Taibah University).
The levels follow the chapter, slide by slide. Each transformation is a weapon: the coach teaches it,
then you shoot the right formula pieces, matrix values and answers as they cross the range.

## Levels (chapter order, 2D only)

| # | Level | Slides | What you shoot |
|---|---|---|---|
| 1 | Pipeline | 3-4 | Local / World / Camera / Screen space and the three transforms |
| 2 | Overview | 5-6 | Which of the five transformations does what |
| 3 | Matrix basics | 7 | A + B, A - B, k.A, A.v, A.B and B.A (order matters) |
| 4 | Translate | 9-10 | x' = x + tx, y' = y + ty (Slingshot) |
| 5 | Scale | 11-12 | x' = x.sx, y' = y.sy, diagonal matrix (Magnifier) |
| 6 | Rotate | 13-15 | x' = x cos t - y sin t, y' = x sin t + y cos t (Revolver) |
| 7 | Shear | 16-17 | x' = x + shx.y, y' = y + shy.x (Crossbow) |
| 8 | Reflect | 18-21 | x-axis, y-axis, origin, y = x, y = -x (Mirror) |
| * | Whole chapter | all | one problem from each level, in order |

Points are columns and the matrix goes on the left: P' = M . P.

## How to play

1. **Armory**: the wall for the chosen level (formulas, matrix, usual exam traps).
2. **Trainer**: the coach walks through the level step by step with a worked example.
3. **Range**: shoot.
   - Transform levels have three drills: *Full* (build the formula, fill the matrix, calculate x' and y'),
     *Formula only* and *Calculate only*.
   - Cover the wall for double points. Every wrong shot gets a reason from the coach.
4. A level gets a tick when a run reaches 70% accuracy. The end screen names your weakest level and offers the next one in the chapter.

Progress is saved in the browser (localStorage).

## Run it

One static file. Open `index.html` in a browser, or host it with GitHub Pages
(Settings > Pages > Deploy from a branch > `main` / root).

## Ideas for later

- Several vertices at once (shapes as 2 x n matrices)
- Composite transformations and order of multiplication
- Homogeneous coordinates (3 x 3 matrices), inverse transformations
