# Making a spatial heat map in ArcGIS Pro

Do you know that there are two types of heat maps?

The first type is the cluster heat map, which was described in my earlier post:

https://www.linkedin.com/posts/thucdao_heat-map-how-color-may-misinterpret-the-activity-6933570366573342722-jnZE

Now let’s talk about the second one: the spatial heat map. I have made an example of it: a map of snow depth in January in Greater Sudbury.

Unlike a cluster heat map, where each cell reports a numeric count, it is impossible to measure the snow depth of every square meter in Greater Sudbury in order to create a spatial heat map. 
The problem is that if you only get snowfall data collected from 39 weather stations across 22 communities, how can you make a snow depth map of the entire Greater Sudbury?

Here spatial interpolation comes into use. Spatial interpolation is the process of using points with known values to estimate values at other unknown points. 
The two widely used interpolation methods are Inverse Distance Weighting (IDW) and Triangulated Irregular Networks (TIN).

I used the IDW method to create this snow depth map in ArcGIS Pro, a desktop GIS software developed by Esri.
- There are 15 levels of snow depth, from 53 cm to 60.5 cm. Each level is 0.5 cm. The darker the color is, the lower the snow depth is. 
- I did not show the locations of 39 weather stations to make the map neat.
- Magenta dots and yellow names are 22 communities in Greater Sudbury.
- The magenta polygon is the Greater Sudbury boundary.

As you can see, we don’t have a problem with color here because I used a sequential palette, not a diverging palette as in my cluster heat map of Sudbury’s temperature (the link in the beginning of this post).

![](SudburySnow/Snow%20depth%20in%20January%20in%20Greater%20Sudbury,%20made%20by%20ThucDao.png)
