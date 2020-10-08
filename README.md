# Karate Chop Polyhedrons - Bleecker's Method

A very simple implementation based on [Volume increasing isometric deformations of convex polyhedra, by karate chops](https://projecteuclid.org/download/pdf_1/euclid.jdg/1214458323).

We start with a Tetrahedron, and we push each of its edges simultaneously in. New faces emerge and the shape has the same surface area, but larger volume (depends on how deep the chop is).

You can play with the size of the tetrahedron and karate chop using the two slide bars on the top-right.

## How it works?

I manually define the vertices and faces of the shape. Then, given a chop depth, I define a function with one parameter ($\alpha$) that controls the locations of the moved vertices (the middle ones), and returns the surface area. Then I try to find $\alpha$ such that the surface area remains unchanged, compared to chop = 0 (up to some precision), using golden ratio line minimization.

## TODO

- Generalize to more polyhedrons  
