# ship-coordinates-to-routes

## Recipe 0

1. DBSCAN (geographic)
1. Minimum spanning tree

## Recipe 1

1. DBSCAN centers ([sklearn](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html))
1. Delaunay triangulation ([scipy](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.spatial.Delaunay.html))
1. Remove long triangles ([networkx](https://networkx.github.io/documentation/networkx-1.10/reference/algorithms.shortest_paths.html))
1. Trace Shortest path trough triangle network (geographic distance)

Shortest path on sphere? Maybe use trick of two distance-preserving projected worlds side-by-side?

## Recipe 2

1. DBSCAN centers ([sklearn](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html))
1. Delaunay triangulation ([scipy](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.spatial.Delaunay.html))
1. Remove long triangles ([networkx](https://networkx.github.io/documentation/networkx-1.10/reference/algorithms.shortest_paths.html))
1. Trace Shortest path trough triangle network (geographic distance)

## Research

Methods:
https://futuretravel.today/approximating-public-transport-route-from-cloud-of-gps-locations-55651a2865ab
http://geoffboeing.com/2014/08/clustering-to-reduce-spatial-data-set-size/
https://geoffboeing.com/2016/06/mapping-everywhere-ever-been/

Data:
https://github.com/miszu/Public-transport-delays-analysis/blob/master/locations.csv
http://www.aishub.net/
http://marinetraffic.com (livemap station JSON)

Documentation:
https://ipyleaflet.readthedocs.io/en/latest/
