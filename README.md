# Segmentation Guided Scoring of Pathological Lesions in Swines Through Convolutional Neural Networks (ID: 34)

## Code
Our UNet-based model can be found in```code/model.py```. 

Our rule-based classifier is available as a single function in ```code/get_lesion_score_from_segmentation```

## Dataset
### Annotation Process
The experts followed a layer-wise annotation strategy. Thus, each anatomical structure is fully annotated even when covered by others:
<th>
  <p align="center">
    <img src="./imgs/annot.gif" alt="Example" width="75%" height="75%">
    <br>Layers of the annotation process.


### Test Set
Test set with 200 examples (50 for each class) is available with no restrictions [HERE]()
Each example comprises:
- An RGB image (.jpg) with shape WxH
- A stacked segmentation (.npy) with shape WxHxC, where C is the number of segmnetation classes
  
Labels for the pleurisy score task are available in the ```raw_labels.txt``` file.
Examples from the 4 classes are reported:

<table style="width:100%">
    <tr>
        <th>
            <p align="center">
            <img src="./imgs/0.jpg" alt="Example" width="75%" height="75%">
            <br>Class 0 example.
            </p>
        </th>
        <th>
            <p align="center">
            <img src="./imgs/1.jpg" alt="Example" width="75%" height="75%">
            <br>Class 1 example.
            </p>
        </th>
     </tr>
 </table>

<table style="width:100%">
    <tr>
        <th>
            <p align="center">
            <img src="./imgs/2.jpg" alt="Example" width="75%" height="75%">
            <br>Class 2 example.
            </p>
        </th>
        <th>
            <p align="center">
            <img src="./imgs/3.jpg" alt="Example" width="75%" height="75%">
            <br>Class 3 example.
            </p>
        </th>
     </tr>
 </table>



### Train Set
Train set is available for research purposes only upon request. Request must be submitted by an associate or full professor.
If you're a private company and you want to get in touch with us, please refers to the article emails 
