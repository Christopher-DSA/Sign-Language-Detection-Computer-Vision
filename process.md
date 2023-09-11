# Process

## The approach:
We will use a SSD (Single Shot Multibox Detector) and a MobNet. This combo is perfect when keeping speed in mind since sign language can be communicated fairly quickly in realtime.

![image](https://github.com/Christopher-DSA/Sign-Language-Detection-Computer-Vision/assets/132075292/82fe6f81-e442-48ca-9984-5fe0003bc3c8)

### Other Options.
-We could have gone with a VGG16 nerual network and while it would likely give better inferences it would also be slower than mobnet which isn't ideal for our real-time sign language detection.
-We also could have gone with ResNet but in this case we are only trying to detect a single persons sign lanaguage and resnet may be too powerful for a simpler task like this, not to mention that we would need
to consider the speed tradeoff that going with this powerful network would bring.

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
