# image_segmentation

impimentation of different segmentation techinques like Region-Based Segmentation, Edge Detection Segmentation, Segmentation based on Clustering, etc in order to understand how image segmentation work.

|Algorithm|Description|Advantages|Limitations|
|:---:|:---:|:---:|:---:|
|Region-Based Segmentation|Separates the objects into different regions based on some threshold value(s).|a. Simple calculations<br>b. Fast operation speed<br>c. When the object and background have high contrast, this method performs really well|When there is no significant grayscale difference or an overlap of the grayscale pixel values, it becomes very difficult to get accurate segments.|
|Edge Detection Segmentation|Makes use of discontinuous local features of an image to detect edges and hence define a boundary of the object.|It is good for images having better contrast between objects.|Not suitable when there are too many edges in the image and if there is less contrast between objects.|
|Segmentation based on Clustering|Divides the pixels of the image into homogeneous clusters.|Works really well on small datasets and generates excellent clusters.|a. Computation time is too large and expensive.<br>b. k-means is a distance-based algorithm. It is not suitable for clustering non-convex clusters.|
|Mask R-CNN|Gives three outputs for each object in the image: its class, bounding box coordinates, and object mask|a. Simple, flexible and general approach b. It is also the current state-of-the-art for image segmentation|High training time|
