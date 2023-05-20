# MultiHealth: Multi-Dimensional Urban and Environmental Exposures and Inequality for Health in Multiple Cities

| Week | Progress |
|----------|----------|
| 19  | |
| 20  | |


Week 19 (8/5 - 14/5):

During this week I’ve worked on the project from Wednesday onwards, due to classes on Monday and Wednesday and assignments for the Data Intensive Systems course, during my work on the project this week I have primarily focused on calculating the distance from the grid centroids to POIs such as bus stops.

However, I have been struggling with extensive run times due to hardware limitations and the large scale of the calculations. Initially, this made it nearly impossible to write and experiment with code since running each iteration could take days. Thus, I've temporarily solved this by extracting a subsection of the population grid data through coordinates, this can be found in the ‘extract.ipynb’ notebook. I have also tried running the code in Google Collab but so far this hasn’t produced any major improvements in running time compared to my personal hardware, although I will continue experimenting with both this option and the possibilities of multiprocessing during the weekend.

Nevertheless, despite the setbacks due to the hardware limitations I have still been able to perform some distance calculations. Firstly, I tried to perform distance calculations based on Manchester’s street network obtained from OSM, however, this proved to be extremely hardware intensive with even a dataset of only 120 grids taking more than five minutes to run. Furthermore, the output consisted of the number of nodes that the route passes between the centroid and the bus stop rather than the total distance. This can be severely inaccurate since it just sees the end of a road as a node, meaning that one five-kilometer-long road could count as one node while four turns within a short distance can count as four nodes. Making the number of nodes a highly unreliable source for determining distance.

So far I haven’t been able to calculate the total route distance in meters while also following the street network, however, I have been able to calculate the Euclidean distance between the centroids and bus stops in meters. Additionally, the Euclidean distance also took significantly less time to calculate, with the runtime of 120 grids decreasing from more than five minutes to less than three seconds. In total, calculating the Euclidean distance for all 246,507 grids took roughly 48 minutes.

The code for calculating the distance through the street network nodes can be found in the 'distcalculation_old.ipynb' notebook.
