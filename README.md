## AIM:
The aim of this project was to detect human faces from an image and group them based on visual similarity using colour-based features. The idea was to explore how simple image features like Hue and Saturation can be used to cluster faces and also match a new template face with existing clusters. 

## METHODOLOGY:
First, faces were detected from the group image using the Haar Cascade classifier in OpenCV. Each detected face region was then converted into the HSV colour space and its average Hue and Saturation values were calculated as features. These features were used as input to the K-Means clustering algorithm to group similar faces together.
A separate template image (Dr. Shashi Tharoor) was also processed in the same way, and its feature values were used to predict which cluster it belongs to. The final results were visualised using scatter plots, centroids, and face thumbnails placed on the graph. 

## KEY FINDINGS:
The clustering successfully grouped faces that had similar colour tones and lighting conditions. Even though the model used very simple features (Hue and Saturation), it was still able to create meaningful visual groupings.
The template image of Shashi Tharoor was correctly mapped to the closest cluster based on similarity, showing that distance-based clustering can be used for basic face grouping tasks. 

## CONCLUSIONS:
This project demonstrates a complete pipeline of face detection, feature extraction, clustering, and classification. It shows that even basic colour features can be useful for grouping images, although for more accurate face recognition, advanced features like deep learning embeddings would be needed.
Overall, the experiment helped in understanding how computer vision and unsupervised learning techniques can be combined for practical image analysis tasks. 


![Face Detection Output](images/result1.png)
![Clustering Plot](images/result2.png)
![Centroid Visualization](images/result3.png)
![Template Mapping](images/result4.png)
![Final Output](images/result5.png)



