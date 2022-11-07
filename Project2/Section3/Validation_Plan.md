# FDA  Submission

**Your Name: DUC_HUY Company

**Name of your Device: HippoVolumeAIQuantification

## Algorithm Description 

### 1. General Information

**Intended Use Statement:** 

For assisting the radiologist to automatically labeling and measuring hippocampal volumes.

**Indications for Use:**
- Patient age >20
- Image charateristics (image modality: MRI and body part: head).

**Device Limitations:**
- Slow performance without GPU
- Other diseases may affect the hippocampal volume.

### 2. Algorithm Design and Function


**Preprocessing Steps:**
- rescale of 1. / 255.0
- Normalization by mean = 0 and std = 1

**CNN Architecture:**

Our CNN architerure is based on the Unet CNN.

**Algorithm performance:**

The algorithm performance is measured based on:
- Dice score
- Jaccard score

### 3. Algorithm Training

**Parameters:**
* Batch size = 8
* Optimizer learning rate = 0.0002
* patch_size = 64


### 4. Databases

The ground truth should be manually labeling by the radiologists. This dataset is stored as a collection of NIFTI files, with one file per volume, and one file per corresponding segmentation mask. The original images here are T2 MRI scans of the full brain. As noted, in this dataset we are using cropped volumes where only the region around the hippocampus has been cut out. 



