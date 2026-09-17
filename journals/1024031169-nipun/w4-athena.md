# Week 4 — 2D Campus Navigation and Route Calculation

## Problem / Challenge

After completing the initial database and repository setup, the next development task was to begin implementing the campus navigation component of Athena.

The objective was to create an initial 2D representation of the campus and allow navigation between different campus locations.The main challenge was that simply assigning coordinates to locations is not sufficient for navigation. A system was also required to represent the actual connections between locations.

Therefore, the navigation system needed to be represented as a graph rather than calculating a direct line between two locations.

## Problems Faced
> Direct Diagonal Route Display

During route visualization, a direct line could be drawn between two locations.

Conceptually:
```javascript
Start
   \
    \
     \
      Destination
```

This does not represent the actual route that a student, cyclist or vehicle can follow.

The problem occurred because the visualization was based directly on the start and destination coordinates instead of following intermediate nodes in the graph.

## Solution

The 2D navigation system was developed by defining:

1. Campus locations.
2. Coordinates for each location.
3. Connections between valid locations.
4. Distance values for connected locations.
5. A route calculation mechanism.
6. A method for displaying the calculated route on the map.

The structure allows the navigation system to determine which locations are directly connected.
