# Hand Gesture Recognition + Segmentation(2nd Project)

This is an extension to the previous project based on Machine learning. In this project, I incorporated a segmentation approach by applying the MaskRCNN segmentation model along with transfer learning based VGG16, InceptionV3 and RESNET50 models. Remarkable accuracy of 97.87%, 98.08%, and 97.46% respectively were achieved.  
 
## Requirements
### Install Required Libraries

```bash
   pip install tensorflow==1.13.1
```
```bash
   pip install keras==2.1.0
```
```bash
   pip install opencv-python
```
```bash
   pip install numpy 
```
```bash
   pip install pandas
```
```bash
   pip install matplotlib
```
```bash
   pip install scikit-learn
```
## Procedure
- First, a part of the dataset containing Orignal Images were labbeled using VGG annotator tool(https://www.robots.ox.ac.uk/~vgg/software/via/via.html) and the label info or the labelled dataset was stored in (.json) format as shown in Sample Images/Label Images.
- Second, MaskRCNN was trained using Train_MaskRCNN.ipynb on the labelled dataset and then implemented using Predict_MaskRCNN.ipynb to segment out the gestures from the rest of the images as shown in Sample Images/Segmented Images.
- Third, by using RESNET50+INCEPTIONV3.ipynb and VGG_16 .ipynb you can perform the real time analysis for Hand Gesture Recognition and can predict the four gestures(Victory, Thumb, Fist, Palm).<br /><br />
**NOTE :-**
**Files used to train and implement MaskRCNN model are present in mrcnn directory** 
