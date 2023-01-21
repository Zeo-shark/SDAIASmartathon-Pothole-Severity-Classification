# Smart-Pothole-Severity-Classification
 
 We have developed a smart solution for pothole detection and classifying the severity in real-time. We tried to use 2D and 3D-based reconstruction techniques for estimating the dimensions of the potholes (the region of interest) and then taking into account the severity index. Since we are using monocular camera-based image frames for pithole classification, the exact 3D reconstruction of the images isn't possible, rather, we are trying to reconstruct a partial or pseudo-3D image of the potholes using a structure-to-motion-based approach of the 2D point clouds formed.

For detecting and extracting the exact area of interest, we have manually segmented and annotated our dataset for the potholes and then used a Detectron 2.0 based image segmentation model for transfer learning that accurately detects the potholes, segments the region of interest, and assigns a confidence score for the detection. We have then extracted the segmented images
