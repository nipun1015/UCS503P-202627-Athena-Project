# Week 5 — Project Prototype Report and 2D Navigation Development

## Problem / Challenge

This week, the development work focused on the map navigation of the Athena project. It was continuing the 2D campus navigation system, where problems were still occurring while finding valid routes between some locations.

The main navigation challenge was that the shortest-path algorithm could calculate a route only when the locations and road connections were correctly represented. Some start-to-destination combinations were still producing incorrect or unavailable routes.

## Problems Faced

Incorrect Route Detection for Some Locations
```text
Uncaught TypeError: Cannot read properties of undefined (reading 'push')
    at connectRoads (script.js:XXX)
    at script.js:XXX
    at script.js:XXX
```
While testing the navigation system, some start-to-destination combinations were still not producing the expected route.

The earlier implementation had coding issues in the road-node and location connections. For example, the road graph contained connections based on the previous node structure, while the road-node coordinates and location mappings were later changed.

This resulted in incorrect or missing paths for some locations.

The issue was therefore not only with the shortest-path calculation itself, but also with how the campus roads and locations were connected in the graph.

## Solution

For navigation, the implementation was modified to use a road-network graph instead of directly connecting the starting and destination coordinates.

The shortest-path approach was then used to calculate a route through the available road nodes.

