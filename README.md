HexaMoon v0.1
=============

Hexagonal Grid Library for Lua

This library is written in PURE Lua, which means it can be used with any framework :D

This library implements Axial Coordinate hex grids with the hexagon oriented such that it is "pointy topped".

What is axial coordinates
-------------------------

In axial coordinates, there are two axes x and y. In my implementation of hex grids, hex coordinate x is aligned with the horizontal coordinate, and hex coordinate y is angled 30 degrees from the vertical coordinate.

Demo
----
See the demo folder.

Functions
---------

A list of functions in the library.

Prefix the functions with what you named the library (i.e., if you did "HXM = require 'HexaMoon", prefix the functions with "HXM.")

###getHexVertices(rad, cx, cy)

Gets the coordinates of the hexagon vertices

* rad - The distance from the center to a corner
* cx - The x-coordinate of the center
* cy - The y-coordinate of the center

###createRectGrid(width, height, obj)

Creates a rectangular shaped grid

* width - The width of the grid
* height - The height of the grid
* obj - The object containing any required variables

###createRhombusGrid(width, height, obj)

Creates a rhombus shaped grid

* width - The length of a row of the grid
* height - The height of the grid
* obj - The object containing any required variables

###getCoordinates(rad, x, y, ox, oy)

Gets coordinates of a hexagon in a axial-coordinate grid

* rad - Radius of a hexagon
* x - The x coordinate
* y - The y coordinate
* ox - The offset x
* oy - The offset y

###drawRectGrid(grid, drawFunction, radius, ox, oy, args)

Draws a rectangular shaped grid (so you don't have to do it yourselves)

* grid - The axial-coordinate grid
* drawFunction - The drawing function. Must take arguments radius, vertices, grid object and the args table for any other optional arguments
* radius - The radius of a hexagon
* ox - The offset x
* oy - The offset y
* args - A table containing optional arguments

###drawRhombusGrid(grid, drawFunction, radius, ox, oy, args)

Draws a rhombus shaped grid

* grid - The axial-coordinate grid
* drawFunction - The drawing function. Must take arguments radius, vertices, grid object and the args table for any other optional arguments
* radius - The radius of a hexagon
* ox - The offset x
* oy - The offset y
* args - A table containing optional arguments

License
-------

Hexagonal Grid Library for Lua
Copyright (C) 2013  Phoenix Enero

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.