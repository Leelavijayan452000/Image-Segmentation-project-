# Image-Segmentation-project-

![ChatGPT Image Apr 13, 2025, 03_44_09 AM](https://github.com/user-attachments/assets/15617c68-eda2-4caa-9794-946d7c9dc31d)

-> Used LandCover.ai dataset with high-resolution aerial images and masks.

-> Split images into 256×256 patches and removed unwanted data background-only patches and kept only useful ones.

-> Normalized image pixel values to the 0–1 range and converted masks into categorical format using onehot encoding.

-> Applied data augmentation: flipping, rotating, brightness adjustment, and zooming then process  data generator to feed batches of augmented data during training.

-> Built the segmentation model using DeepLabV3+ architecture. Integrated ASPP for multi-scale context extraction and used ResNet-50 as the backbone for feature extraction.

-> Trained the model using Focal Loss and Jaccard Loss with Adam optimizer then used callbacks to improve training performance. Validated model using IoU and pixel accuracy.

-> Merged segmented patches to reconstruct full images then applied smoothing to improve the final segmentation output.

-> Segmented images into classes: Road, urban, Water, and Forest. and pixel count for each class to calculate percentage coverage.

-> Visualized results with a pie chart showing land cover distribution

![Poster](https://github.com/user-attachments/assets/73c4c44e-ed84-45df-baf3-eac8e31da2b9)







