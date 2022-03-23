## :microscope: Extracting Metadata from 3D Sea Urchin Trabecular Bone Structure

### Steps:
![](/images_and_gifs/horizontal_skeletonization_steps.png)
1. Blur raw data to smooth out high freuency noise -> leads to better thresholding results
2. Threshold image to convert grayscale image(s) into binary format in relation to the threshold value.
3. Skeletonize image (using Lee94 algorithm):
4. Distance Transform (2D or 3D) - labels each pixel/voxel of the image with the distance to the nearest background/void.
5. Extract Nodes and Branches
6. Export data as CSVs
### :wrench: Testing on One 2D slice:
<img src="/images_and_gifs/processing_steps.gif" width="750" title="hover text">
 
### :mag_right: Zooming In:
<img src="/images_and_gifs/lee94_skeletonization.gif" width="750" title="hover text">
 
<img src="/images_and_gifs/centroids_and_pore_perimeters.gif" width="750" title="hover text">

### :rocket:	Skeletonize 3D Data:
The gif below showcases z axis slices - from left: thresholded data, 3D distance transform (distances mapped as pixel values), branch pixels, node pixels.The 3D skeleton might look bizare when viewed one slice at a time, but makes much more sense when viewed in 3D. This skeleton data would later be used to run mechanical simulations.

<img src="/images_and_gifs/horizontal_seg+distrans+branch+nodes.gif" width="750" title="hover text">

### Thresholded data and Skeleton:

![](/images_and_gifs/raw_data_3d_imjoy.gif)
![](/images_and_gifs/skeleton_3d_imjoy.gif)




 



