# U-Net Image Segmentation

This project implements an image segmentation task using a U-Net model. The goal is to segment images of horses from a dataset, and the provided code accomplishes this by following a series of steps:

1. **Data Preparation**
   - Download and unzip the COCO dataset annotations.
   - Create directories for training and validation images.
   - Fetch and filter the dataset to obtain images and annotations specific to the "horse" category.

2. **Mask Generation**
   - Generate segmentation masks for the training and validation sets based on the filtered annotations.
   - These masks are binary masks that highlight the region where the "horse" objects are located in the images.

3. **U-Net Model**
   - Implement a U-Net architecture for image segmentation.
   - Define the UNet class, which includes an encoder and a decoder.
   - Set up data loading and preprocessing for training and validation sets using a custom dataset class.
   - Train the U-Net model on the horse segmentation task.

4. **Evaluation**
   - Evaluate the trained model on a sample image.
   - Display the original image, predicted binary mask, and the binary mask thresholded at 0.5.
