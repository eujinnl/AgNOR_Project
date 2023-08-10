Task: group of images have AgNOR cells and need to be labelled
__
Solution Outline:
![image](https://github.com/eujinnl/AgNOR_Project/assets/128717520/49edabf5-c149-4816-9677-abfdf4dd712b)
__
Details:
A pre-trained RetinaNet model as the backbone for the object detector. Image classificator's model summary is as following: __
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 32, 30, 30]             896
              ReLU-2           [-1, 32, 30, 30]               0
           Dropout-3           [-1, 32, 30, 30]               0
            Conv2d-4           [-1, 32, 30, 30]           9,248
              ReLU-5           [-1, 32, 30, 30]               0
         MaxPool2d-6           [-1, 32, 15, 15]               0
            Conv2d-7           [-1, 32, 15, 15]           9,248
              ReLU-8           [-1, 32, 15, 15]               0
         AvgPool2d-9             [-1, 32, 7, 7]               0
          Flatten-10                 [-1, 1568]               0
           Linear-11                  [-1, 512]         803,328
             ReLU-12                  [-1, 512]               0
          Dropout-13                  [-1, 512]               0
           Linear-14                   [-1, 12]           6,156
================================================================
Total params: 828,876
Trainable params: 828,876
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.01
Forward/backward pass size (MB): 1.30
Params size (MB): 3.16
Estimated Total Size (MB): 4.47
----------------------------------------------------------------
