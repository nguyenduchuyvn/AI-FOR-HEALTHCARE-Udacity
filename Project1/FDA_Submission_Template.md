# FDA  Submission

**Your Name: DUC_HUY Company

**Name of your Device: AI for Pneumonia Detection from Chest X-Rays

## Algorithm Description 

### 1. General Information

**Intended Use Statement:** 

For assisting the radiologist into Pneumonia detection on chest x-rays.

**Indications for Use:**
- Use in chest x-rays screenings studies
- Use in women and men with ages less than 88 years.

**Device Limitations:**
- Slow performance without GPU
- The algorithm is not tested for patients with previous history of Pneumonia.

**Clinical Impact of Performance:**
- We set our threshold in function of maximizing the F1 score
![fig](./roc.png "F1 Curve")


### 2. Algorithm Design and Function

<< Insert Algorithm Flowchart >>

**DICOM Checking Steps:**

**Preprocessing Steps:**
- rescale of 1. / 255.0
- Normalization by mean = 0 and std = 1

**CNN Architecture:**

Our CNN architerure is based on the VGG16 CNN with freezing all but the 2 last convolutional layer of VGG16 and adding Flatten() - (Dense(1, activation='sigmoid').

### 3. Algorithm Training

**Parameters:**
* Types of augmentation used during training: rescale of 1. / 255.0, horizontal_flip, height_shift_range of 0.1, width_shift_range of 0.1, rotation_range of 20, shear_range of 0.1,   zoom_range of 0.5
* Batch size = 128
* Optimizer learning rate = 1e-4
* Layers of pre-existing architecture that were frozen: freeze all but the 2 last convolutional layer of VGG16
* Layers of pre-existing architecture that were fine-tuned: the 2 last convolutional layer of VGG16
* Layers added to pre-existing architecture: Flatten() - (Dense(1, activation='sigmoid')

<< Insert algorithm training performance visualization >> 
![fig](./training.png "training Curve")
<< Insert P-R curve >>
![fig](./F1_figure.png "F1 Curve")

**Final Threshold and Explanation:**

The threshold = 0.15 is selected because of its best F1 scores.

### 4. Databases
 (For the below, include visualizations as they are useful and relevant)

**Description of Training Dataset:** 

The trainning dataset has 2290 records including:
* Positive    1145
* Negative    1145

**Description of Validation Dataset:** 

The validation dataset has 1430 records including:
* Negative    1144
* Positive     286

