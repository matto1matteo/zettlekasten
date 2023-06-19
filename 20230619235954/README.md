# Axis Aligned Boundging Boxes (AABB)

It means that the bounding box used for collisions detection are, yep, boxes
without any orientation

## Point inside AABB

Check wheter or not a point is inside a box

## Two AABB Intersections

Naively, in order for two AABB to intersect, at least two of their side must
intersect.

### Horizontal and Vertical Overlap

Two AABB overlaps if there are both horizontal and a vertical overlap.
