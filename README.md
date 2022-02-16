1. **Blur Raw Data**: to smooth out high freuency noise -> leads to better thresholding results
2. **Threshold image**: to convert grayscale image(s) into binary format in relation to the threshold value.
3. **Skeletonize image (using Lee94 algorithm)**: this method uses an octree data structure to examine a 3x3x3 neighborhood of a pixel. The algorithm proceeds by iteratively sweeping over the image, and removing pixels at each iteration until the image stops changing. 
4. **3D distance Transform**: labels each pixel/voxel of the image with the distance to the nearest background/void.
5. **Nodes and Branches**
6. **Export data as CSVs**


### 2D Example
![](/images_and_gifs/horizontal_skeletonization_steps.png)

### 3D Skeleton
![](/images_and_gifs/3d_skeleton_scatterplot.gif)
