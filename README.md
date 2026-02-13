# MLPR-LAB-5
#Overview
In this lab, we worked on detecting faces from an image and then grouping them using a distance-based clustering approach. The idea was to understand how feature extraction and K-Means clustering work together in a simple computer vision task. We also tested the model by classifying a new template image.

#Aim:
Detect faces using Haar Cascade classifier
Extract basic color features (Hue and Saturation)
Apply K-Means clustering on the extracted features
Classify a new face based on the trained clusters

#Methodology
First, the input image was converted to grayscale and face detection was performed using OpenCV’s Haar Cascade. After detecting the faces, the image was converted into HSV format, and the mean Hue and Saturation values were calculated for each face region.
These feature values were then used as inputs to the K-Means algorithm (k = 2) to form clusters. The cluster centroids were calculated and visualized.
Finally, a template image was processed in the same way and its cluster label was predicted using the trained K-Means model.

#Results
Faces were successfully detected from the given image. The clustering algorithm divided the faces into two groups based on color similarity. The template image was also classified into one of the clusters correctly. The visualization clearly showed the separation of clusters along with their centroids.

#Conclusion
This lab helped in understanding how distance-based classification works in practice. It showed that even simple features like Hue and Saturation can be used for clustering. The experiment also reinforced concepts like feature extraction, clustering, and the importance of choosing appropriate distance measures.
