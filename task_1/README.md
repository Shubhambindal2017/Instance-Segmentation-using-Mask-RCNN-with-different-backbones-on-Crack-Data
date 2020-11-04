# Task 1. Retrain the model

I have trained MASK R-CNN with Resnet101 backbone on cracks dataset using matterport's implenetation, by using transfer learning, as I made use of its pre-trained MASK-RCNN weights trained on COCO dataset.

I used : 

    tensorflow : 1.15.2
    keras      : 2.3.1

Their were only 2 classes, 1 background and 1 crack.

I trained my model on 25 epochs, with each epoch of 300 steps, 300 to get frequent reading from tensorboard, after each epoch
My training gets affected in between, so break/unsual graph can be seen ~10-12 epochs in tensorboard graphs.

I just trained layers starting from resnet4 stage.

I got mAP of 0.204 (as trained just for 25 epochs, each with 300 iterations)

Model is trained for just 25 epochs with each epoch just containing 300 steps, and this problem of crack segmentation is very different from commnon problems in which we have fixed/defined boundaries.
So I think the results are acceptable ones.

Folder :

    gt_images            : contains ground truth masked images
    predicted_images     : contains predicted masked images
    
**[Trained model can be found here](https://drive.google.com/file/d/1-NJLyi6T3uNM-wjJTn3XOyUrZkEztcvw/view?usp=sharing)**
