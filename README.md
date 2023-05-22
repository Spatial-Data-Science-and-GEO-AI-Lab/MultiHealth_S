# MultiHealth: Multi-Dimensional Urban and Environmental Exposures and Inequality for Health in Multiple Cities

| Week | Progress |
|----------|----------|
| 17 | Read provided literature to immerse myself within the topic.
| 18 | Used worldpop data to create 100 by 100 meter population grids of the Greater Manchester area. Furthermore, utilized the Open Street Map Python library 'osmnx' to extract data points such as bus stops, restaurants, shops, and cycle lanes. Additionally, converted both the grid area and data points to the British National Grid (EPSG:27700) so they can be accurately overlaid.
| 19 | Adapted code to calculate the travel distance from the Manchester grid centroids to certain POIs (in this case, bus stops). However, struggled with extensive run times due to hardware limitations and the scale of the calculations. Thus, looked at various possible solutions such as the usage of cloud environments and further code optimizations. |
| 20 | Worked on optimizing the distance code by implementing a threshold of 1000 meters, additionally spent most of the weekend on the removal of the 'for loop' and implementation of 'Numpy Vectorization' to further improve the runtimes. |
