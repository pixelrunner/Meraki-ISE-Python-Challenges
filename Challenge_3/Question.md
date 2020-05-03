# Challenge 3: Spiral Memory

You come across an experimental new kind of memory stored on an infinite two-dimensional grid.

Each square on the grid is allocated in a spiral pattern starting at a location marked 1 and then counting up while spiraling outward. For example, the first few squares are allocated like this:


|         |            |   |            |   |            |   |
| ------------- | ------------- | ----- | ------------- | ----- | ------------- | ----- |
|         | 17      | 16 | 15 | 14 | 13 |         |
|         | 18      | 5      |   4 | 3 | 12 |         |
|         | 19 | 6      |    1 | 2 | 11 |         |
|         | 20 | 7      |    8 | 9 | 10 |         |
|         | 21 | 22      |   23 | ---> | ... |         |
|         |            |   |            |   |

While this is very space-efficient (no squares are skipped), requested data must be carried back to square 1 (the location of the only access port for this memory system) by programs that can only move up, down, left, or right. They always take the shortest path: the [Manhattan Distance](https://en.wikipedia.org/wiki/Taxicab_geometry) between the location of the data and square **1**.

For example:

- Data from square 1 is carried 0 steps, since it's at the access port.
- Data from square 12 is carried 3 steps, such as: down, left, left.
- Data from square 23 is carried only 2 steps: up twice.
- Data from square 1024 must be carried 31 steps.

**How many steps** are required to carry the data from the square **277678** all the way to the access port **(1)**?

-----

# Part 2
OK, so you've worked out the amount of fuel you need and that has been added to your ship.

The Go/No-Go checks can continue, the person in charge of the "Rocket Equation Double-Checker" stops the launch sequence. Apparently, you forgot to include additional fuel for the fuel you just added.

Fuel itself requires fuel just like a module - take its mass, divide by three, round down, and subtract 2. However, **that fuel also requires fuel, and that fuel requires fuel, and so on**. Any mass that would require negative fuel should instead be treated as if it requires zero fuel; the remaining mass, if any, is outside the scope of this calculation.

**So, for each module mass, calculate its fuel and add it to the total. Then, treat the fuel amount you just calculated as the input mass and repeat the process, continuing until a fuel requirement is zero or negative.**

For example:

- A module of mass 14 requires 2 fuel. This fuel requires no further fuel (2 divided by 3 and rounded down is 0, which would call for a negative fuel), so the total fuel required is still just 2.
- At first, a module of mass 1969 requires 654 fuel. Then, this fuel requires 216 more fuel (654 / 3 - 2). 216 then requires 70 more fuel, which requires 21 fuel, which requires 5 fuel, which requires no further fuel. So, the total fuel required for a module of mass 1969 is 654 + 216 + 70 + 21 + 5 = 966.
- The fuel required by a module of mass 100756 and its fuel is: 33583 + 11192 + 3728 + 1240 + 411 + 135 + 43 + 12 + 2 = 50346.

What is the sum of the fuel requirements for all of the modules on your spacecraft when also taking into account the mass of the added fuel? (Calculate the fuel requirements for each module separately, then add them all up at the end.)

Upload your script(s)to github (don't worry if it's part of the "part 1" script), and relax; safe in the knowledge you now have enough fuel to take off.
