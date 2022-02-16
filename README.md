## Extracting Metadata from 3D Sea Urchin Trabecular Bone Structure

### Steps Involved:
![](/images_and_gifs/horizontal_skeletonization_steps.png)
1. Blur raw data to smooth out high freuency noise -> leads to better thresholding results
2. Threshold image to convert grayscale image(s) into binary format in relation to the threshold value.
3. Skeletonize image (using Lee94 algorithm):
4. Distance Transform (2D or 3D) - labels each pixel/voxel of the image with the distance to the nearest background/void.
5. Extract Nodes and Branches
6. Export data as CSVs
### Testing on one 2D slice:
<img src="/images_and_gifs/processing_steps.gif" width="750" title="hover text">
 
### Zooming In:
<img src="/images_and_gifs/lee94_skeletonization.gif" width="750" title="hover text">
 
<img src="/images_and_gifs/centroids_and_pore_perimeters.gif" width="750" title="hover text">

### Skeletonize 3D Data:
This skeleton data would later be used to run mechanical simulations. the gif below showcases z axis slices - from left: thresholded data, 3D distance transform (distances mapped as pixel values), branch pixels, node pixels.

<img src="/images_and_gifs/horizontal_seg+distrans+branch+nodes.gif" width="750" title="hover text">

The 3D skeleton might look bizare when viewed one slice at a time, but makes much more sense when viewed in 3D
![](/images_and_gifs/3d_skeleton_scatterplot.gif)

 



