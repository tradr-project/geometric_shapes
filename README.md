# Geometric Shapes

This package contains generic definitions of geometric shapes and bodies, as well as tools for operating on shape messages.
Shapes represent only the form of an object.
Bodies are shapes at a particular pose. Routines such as point containment and ray intersections are provided.

Supported shapes:
- sphere
- box
- cone
- cylinder
- mesh

Note: Bodies for meshes compute the convex hull of those meshes in order to provide the point containment / ray intersection routines.

Note: There was a recent change in point containment computations - now all bodies are expected to also contain their surface points. [The old behavior was inconsistent](https://github.com/ros-planning/geometric_shapes/issues/91). Rounding errors may still yield surprising results, though.

Note: [shape_tools](https://github.com/ros-planning/shape_tools) package was recently merged into this package

## Build Status

Travis CI: [![Build Status](https://travis-ci.org/ros-planning/geometric_shapes.svg?branch=indigo-devel)](https://travis-ci.org/ros-planning/geometric_shapes)

Devel Job: [![Build Status](http://build.ros.org/buildStatus/icon?job=Ibin_uT64__geometric_shapes__ubuntu_trusty_amd64__binary)](http://build.ros.org/view/Ibin_uT64/job/Ibin_uT64__geometric_shapes__ubuntu_trusty_amd64__binary/)

Debian Job: [![Build Status](http://build.ros.org/buildStatus/icon?job=Idev__geometric_shapes__ubuntu_trusty_amd64)](http://build.ros.org/view/Idev/job/Idev__geometric_shapes__ubuntu_trusty_amd64/)
