# Cornea Iris Dataset
Collected and created by Sarah Barrington, UC Berkeley

## Overview
This dataset contains a sample of irises cropped from the eyes of both real and fake human portraits. The purpose of this dataset is to support research into deep-fake detection through the analysis of the corneal surface of the subject's eye. 

## Data Collection Process
This repository contains one folder of real irises and one folder of deep-fake generated irises. The real portraits were sourced from the Flickr-Faces High Quality (FFHQ) public dataset, and the fakes were generated and scraped via thispersondoesnotexist.com (generated using StyleGAN 2). 

Facial landmarks were automatically extracted via the face_alignment package, and a circle fitted to the corresponding corneal surface keypoints using a total least squares approximation. Each image was then cropped to the corneal region only, encompassing mainly the iris of each eye. Failure cases were manually removed if the subject had their eyes covered (for example, wearing sunglasses) or if the automatic extraction failed (by capturing the iris as less than 50% of the photo). 

## Data Collection Process
All pass cases are contained in labelled folders. Both the original crop sizes (~50x50px) and resized images (512x512px) are included for ease of viewing.  

## Contact
For questions or contact, please email sbarrington@ischool.berkeley.edu. 

