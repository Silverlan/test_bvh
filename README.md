# BVH Construction and Traversal Library

This library is a small, standalone library for BVH construction and traversal. It is licensed
under the MIT license.

## Features

- A high-quality, single-threaded sweeping SAH builder,
- A fast, medium-quality, single-threaded binned SAH builder inspired by
  "On Fast Construction of SAH-based Bounding Volume Hierarchies", by I. Wald,
- A fast, high-quality, multithreaded mini-tree BVH builder inspired by
  "Rapid Bounding Volume Hierarchy Generation using Mini Trees", by P. Ganestam et al.
- A fast and robust traversal algorithm using "Robust BVH Ray Traversal", by T. Ize.
- A fast ray-triangle intersection algorithm based on
  "Fast, Minimum Storage Ray/Triangle Intersection", by T. Möller and B. Trumbore,
- Can be parametrized on the dimension (e.g. 2D, 3D, 4D BVHs are supported) & scalar type
  (e.g. `float` or `double`),
- Only depends on the standard library (parallelization uses a custom thread pool based on
  `std::thread`).

## Usage

![simple example](https://github.com/madmann91/bvh/blob/v2/test/main.cpp)
