Trains
======

Single/Double Headed
--------------------

.. images:: images/factorio-double-vs-single-headed-trains.jpeg
   :width: 600

Train networks are generally designed around either single or doubled headed trains. While possible to combine this is less common.

Single headed trains only travel is on direction. Trains therefore require more space to turn around and travel in loops. Convention is to build an even number (usually 2) of parallel rails where for each rail, trains only travel in a single direction.

Double headed trains can travel in both directions. These networks generally require less space but can be more difficult to accommodate multiple trains on a single track.

LHD/RHD
-------

Refers to trains traveling on the "Right" vs. the "Left" hand side of parallel tracks. Designing such that trains only travel a single direction on a rail (exactly which, left vs. right, is arbitrary) is ubiquitous and generally considered a mandatory design simplification.

Configurations
--------------

Trains are generally discussed using the X-Y notation, where X is the number of engines, and Y is the number of wagons. Bases will typically use only a small number of unique configurations to simplify the design.

The most common train is 1-4. This offers a nice balance between design difficulty and throughput. Players will often use 1-4 in conjunction with 1-2 for lower throughput use cases like oil.

As the number of wagons increases, the number of engines necessarily increases for breaking and acceleration. 2-8 is next common size up.

Intersections
-------------

.. note::
    To simplify, we discuss intersections in the context of RHD. Everything is reversed for LHD.

Intersecting rails is a key design challenge. A primary debate is whether to allow left turns.

Roundabouts
```````````

Roundabouts are the simplest and most beginner friendly intersections. The ability for a train to turn around can be a huge simplifier.

These are not used in larger bases partially because their proclivity to deadlock without great care, but mostly because loops incur a much higher UPS penalty during train pathfinding.

Left turns
``````````

For non-roundabout intersections (3 and 4 way), players have a decision to allow or disallow left turns.

Left turns will generally cause trains to stop more, because the block more: They block oncoming trains going straight or right (and trains coming from the left turning left).

Whether this has a noticable impacts depends on several factors, such as network congestion and fuel (speed/acceleration).

Stackers
--------

To minimize downtime while trains travel between stations, "stackers" enable multiple trains to wait at both pickup and dropoff locations. Stackers are used in conjunction with train limits to optimize throughput.
