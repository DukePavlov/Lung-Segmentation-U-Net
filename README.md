# Lung-Segmentation-U-Net
### Semantic segmentation on Lung X-Ray images, done by U-Net

### This notebook covers The augmentation, training/evaluation and testing of U-Net architecture model for semantic segmentation on dataset retrieved from Kaggle.
#### The pipeline is written using pytorch, opencv and augmentations were done via albumentation library.
#### Beside just using models result. Image processing has been done in order to get improve results. 
#### Dataset has been cleaned manually and programatically(This was done in script outside the main notebook("Lung_segmentation_Notebook")
#### Early stopping with patientce 20 was being used as additional regularization technique; Adam optimizer, Cross_entropy_loss as a loss function, BinaryJaccardIndex as an accuracy metric and learning rate was set to 1e-4. 
#### Due to lack of resources(quite long training at the time) training was executed in 40 epochs multiple times, and the results of each epoch has been saved in a dict for review when the results get high enough or to finish due to early stopping.
