To increase our storage capacity we should start with calculating the area of the rooms we have available.

You should write a function to calculate the area of simple figures: circles, rectangles and triangles.
You are give an arbitrary number of arguments which the function should use to calculate the area for the different figures.

- One argument -- The diameter of a circle and you need calculate the area of the circle.
- Two arguments -- The side lengths of a rectangle and you need calculate the area of the rectangle.
- Three arguments -- The lengths of each side on a triangle and you need calculate the area of the triangle.

The result should be given with two digit precision like so: +-0.01

![Simple areas](simple-areas.svg)

**Input:** One, two or three arguments as floats or as integers.

**Output:** The area of the circle, the rectangle or the triangle as a float.

**Example:**

```python
simple_areas(3) == 7.07
simple_areas(2, 2) == 4
simple_areas(2, 3) == 6
simple_areas(3, 5, 4) == 6
simple_areas(1.5, 2.5, 2) == 1.5
```
**How it is used:**

Python can be an useful tool for mathematics and science due to its simplicity, readability and ease of use.


**Precondition:**

```python
0 < len(args) <= 3
all(0 < x <= 1000 for x in args)
```

For the "triangle" cases, the sum of the lengths of any two sides always exceeds the length of the third side.

