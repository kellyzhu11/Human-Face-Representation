# Human Face Representation Using PCA and Autoencoder
This project was part of my work for UCLA STATS M231/CS276 (Pattern Recognition and Machine Learning) during fall 2018. The purpose of this project is to compare two types of human face representations in the context of dimension reduction: PCA and Autoencoder. Active Appearance Model (AAM) is applied to represent and reconstruct faces.

## Dataset
The CelebA dataset contains 1000 face images cropped to 128 × 128 pixels by the OpenFace. The face images are pre-processed so that the background and hair are removed. Each face has a number of landmarks, 68 points per image, which are identified by OpenFace. These landmarks should be aligned so that the appearance (i.e. grey level, intensity on pixels) can be compared meaningfully across face.

## Usage
### Clone the repositories
 
 ```bash
 git clone https://github.com/kellyzhu11/Human-Face-Representation.git
 ```
 
### Get Face Representations by PCA
run pca.ipynb
### Get Face Representations by Autoencoder
run autoencoder.ipynb

## Results
Original test images
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/origin.png" width =400/>
</p>

### PCA
#### Reconstruction
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/pca_reconstruction.png" width=400/>
</p>

#### Ramdom faces
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/pca_random_face.png" width=400/>
</p>

### Autoencoder
#### Reconstruction
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/ae_reconstruction.png" width=400/>
</p>

#### Latent Space Exploration
Latent space for landmarks

First dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/lm_d1.png" width=700/>
</p>
Second dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/lm_d2.png" width=700/>
</p>
Thrid dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/lm_d3.png" width=700/>
</p>
Fourth dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/lm_d4.png" width=700/>
</p>

Latent space for appearance

First dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/ap_d1.png" width=700/>
</p>
Second dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/ap_d2.png" width=700/>
</p>
Thrid dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/ap_d3.png" width=700/>
</p>
Fourth dimension: 
<p align="center">
  <img src="https://raw.githubusercontent.com/kellyzhu11/Human-Face-Representation/master/pics/ap_d4.png" width=700/>
</p>
