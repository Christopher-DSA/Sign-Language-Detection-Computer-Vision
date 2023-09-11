# Process

## The approach:
We will use a SSD (Single Shot Multibox Detector) and a MobNet. This combo is perfect when keeping speed in mind since sign language can be communicated fairly quickly in realtime.

![image](https://github.com/Christopher-DSA/Sign-Language-Detection-Computer-Vision/assets/132075292/82fe6f81-e442-48ca-9984-5fe0003bc3c8)

### Other Options.
-We could have gone with VGG 16 or Res Net for the base network, however keeping in mind that this is a real-time applciation we are going to go with mobnet which is more light-weight and speedy.
-Instead of SSD we could have gone with YOLO (you only look once) since it is also quite fast when it comes to object recognition
,however yolo can struggle with more intricate differences in hand gestures or changes in a scene in general so we will go with SSD.

---
- Collect Images to feed the machine learning model. These images will be of the following hand signs: hello, no, yes, thankyou.
- Label the images so we can tell the computer what the right answers are. (Supervised Learning)
- Split the images into training and testing splits.
- Create TF record
- Train the model with tensor flow mob net ssd network.
- Run 10000 cycles untill we minimize the loss of the model.
- Test the model.
- Tuning the model by making adjustments.
- Retrain.
- Complete!
