# Human-Face-Reprsentation-Using-PCA-and-Autoencoder
This project was part of my work for Advanced Digital Image Processing at the University of Iowa during spring 2017. 
## Description
Human face is a very important pattern and has been extensively studied in the past 30 years in vision, graphics, and human computer interaction, for tasks like face recognition, human identification, expression, animation etc. An important step for these tasks is to extract effective representations from the face images. This project will compare two types of representations in the context of dimension reduction: PCA (Linear) and Autoencoder (non-linear)

## Dataset
We used the CelebA dataset containing 1000 images cropped to 128 × 128 pixels by the OpenFace. The face images are pre-processed so that the background and hair are removed. Each face has a number of landmarks, 68 points per image, which are identified by OpenFace. These landmarks should be aligned so that the appearance (i.e. grey level, intensity on pixels) can be compared meaningfully across face.

## Active Shape Model (ASM) and Active Appearance Model (AAM)
### ASM

The ASM model is trained from manually drawn contours (a set of "landmark" points) in training images. It is used for representing the shape of objects.

### AAM:
The AAM model consists of a shape model (i.e. ASM) and a appearance model. After finding the shape model, all training data objects are deformed to the mean shape. Then the appearance model is used to represent the appearance of objects. By fitting a parametric representation of a certain object through optimization, we can reconstruct or generate new object.

In this project, we use PCA and Autoencoder to build the ASM model and AAM model.
