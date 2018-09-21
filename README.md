# Sampling-Based Mobile Robot Path Planning Algorithm by Dijkstra, Astar and Dynamic Programming

In this repository, we briefly presented full source code of Dijkstra, Astar and Dynamic Programming approach to find best route from starting node to end node on 2D graph. We also provide a main script which performs these algorithms on given map.

## Map Definiton
We already provide a sample map creatin in map_definition.m source code. We defined all closed polygon in that maps which shows the obstacles. In sample map, there are 13 different obstances whose edges are defined by given x and y coordinates. One sample is shown by followings;
```
map.pgx{1}=[2 8.5 8.5 4 2 2 1 1 2 4 2];
map.pgy{1}=[8 10 1 3 3 1 1 6 6 5 8];
```
You can add new obstacles or modify the given obstacle to create your own map. 

## Sampling-Based Path Planning
In sampling based method, we need to generate some certain number of points on to the map which are fall into non occupied region of given map. Then we calculate which node has connection to which nodes. By this way, we obtain the undirectioned graph of generated random points. To generate that points, we can use some sophisticated method to distirbute the nodes all around the map as clever as possible. But in that repository we selected to generate them by just uniformly random. We generated 100 number of nodes which are on the free region of map. there is the given map, generated nodes and their connections.

<p align="center">
  <img src="Output/map.jpg" width="300"/>  
  <img src="Output/map_nodes.jpg" width="300"/>  
</p>
