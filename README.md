# CLIP-vs-HOG
comparaison between the two models
# Presentation of the two compared approaches:
# Introduction:
Describing regions of interest in images is important to many computer vision tasks, including
object detection and content-based image retrieval (CBIR). Two distinct approaches for achieving this
are Histograms of Oriented Gradients (HOG) and Contrastive Language-Image Pretraining (CLIP).
While HOG is a traditional feature descriptor focusing on structural patterns, CLIP uses deep learning
to understand content. This section compares these two methods in terms of their principles.


# Histograms of Oriented Gradients (HOG):
The Histogram of Oriented Gradients (HOG) is a widely used feature descriptor in the fields of
computer vision and image processing. It examines the distribution of edge orientations within an
object to characterize its shape and visual characteristics. The HOG technique entails calculating the
gradient magnitude and orientation for every pixel in an image, followed by segmenting the image
into smaller cells.
![image](https://github.com/user-attachments/assets/e47e9f01-bb67-40bd-9049-609b20314321)





# Contrastive Language-Image Pretraining (CLIP):
CLIP is a deep learning model that aligns images and textual descriptions into a shared space,
enabling tasks like image description, retrieval, and classification.
This model can understand both text descriptions and images by utilizing a training method that fo-
cuses on contrasting pairs of text and images.

![image](https://github.com/user-attachments/assets/459866aa-503e-4ef4-880f-4294a786e739)
![image](https://github.com/user-attachments/assets/189411c7-8ee4-475e-8561-9868921be1d6)
# Comparison:
![image](https://github.com/user-attachments/assets/3e2a4148-134b-4aba-9247-3ee9fae99a12)
The results support the hypotheses regarding sensitivity to noise, object structure, and bounding
box effects. HOG-based similarity is more affected by noise than CLIP, as evidenced by its lower and
more inconsistent similarity scores, confirming that HOG relies heavily on edge-based features while
CLIP maintains robust performance due to its semantic understanding. Additionally, HOG demon-
strates greater sensitivity to object structure changes, with noticeable drops in similarity for objects
with less defined edges, whereas CLIP remains stable. The bounding box hypothesis is also validated,
as HOG similarity varies significantly with cropping and misalignment, while CLIP remains consis-
tent. However, certain cases, such as "pickles" exhibit mixed behavior, suggesting the need for more
controlled tests. To improve these evaluations, systematic noise levels, structured shape variations,
and a bounding box ablation study could be implemented to better quantify their effects.




