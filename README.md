# Tube Map
SVG Tube map and journey planner with synesthetic details of tastes

I couldn't find an SVG tube map, even though it is a classic of angular graphic design. So, I made one.

Rather than draw it out by hand, the lines and stations are described as JSON objects in the data directory. This includes details of which direction the station tick marks should move in, interchanges and linked stations, and where to place labels.

This map is made up of:
 - Lines - which define the colours to be used, and have a route
 - Routes - which are made up of linked pairs of stations and define where you can go
 - Stations - which can belong to many lines or routes

In order to draw bends in the line (and Thames) where there is no station, there are "virtual stations". These are used for route finding but not marked with map symbols.

Lines are drawn by following each line's route with the appropriate colours. The routing details are also used for pathfinding. When using the route planner, it identifies a new sub-route and shades out the other parts of the map.

There is also an option to convert the map to food tastes reported by a synaesthetic man who visited all of them. This was to show it worked when changing the text, and because it was interesting.

Idea for future expansion: other data sets that could be applied to the name, like The Great Bear (https://en.wikipedia.org/wiki/The_Great_Bear_(lithograph))
