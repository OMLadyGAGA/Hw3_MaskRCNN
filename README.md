# Hw3: Mask R-CNN for Object Detection and Segmentation


In this Assignment, I follow [this post](https://github.com/matterport/Mask_RCNN?fbclid=IwAR2LkSVtpX0zl_WczTFgjdWAbzfftV1qrwAo8V8BQTwoeb8KDgs3rw3dUeE) to finish Hw3. I modified some part of code in order to train hw3's dataset.


```
# Train a new model starting from pre-trained COCO weights
python3 samples/coco/coco.py train --dataset=/path/to/coco/ --model=coco

# Train a new model starting from ImageNet weights

python3 samples/coco/coco.py train --dataset=/path/to/coco/ --model=imagenet

# Continue training a model that you had trained earlier

python3 samples/coco/coco.py train --dataset=/path/to/coco/ --model=/path/to/weights.h5


# Continue training the last model you trained. This will find

# the last trained weights in the model directory.
python3 samples/coco/coco.py train --dataset=/path/to/coco/ --model=last
```

I use second instruction to train the dataset this course provided. According to the [this post](https://github.com/matterport/Mask_RCNN?fbclid=IwAR2LkSVtpX0zl_WczTFgjdWAbzfftV1qrwAo8V8BQTwoeb8KDgs3rw3dUeE) second instruction able to exploit imagenet weight to train custom dataset.
