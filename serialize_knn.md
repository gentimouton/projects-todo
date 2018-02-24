
serialize (and possibly compress) a k-nearest neighbor model (ie store/load)
- some possible heuristics: if all the neighbors of a point have that point's color, remove that point
- use [fortune's algo](https://en.wikipedia.org/wiki/Fortune%27s_algorithm) to voronoi (n log n) - also [in python](https://github.com/jansonh/Voronoi)
- lossless vs lossy compressions?
- is knn appropriate when high dimensions? reduce dimensions first?
- see also the [boost polygon library for voronoi](http://www.boost.org/doc/libs/1_63_0/libs/polygon/doc/voronoi_main.htm)
