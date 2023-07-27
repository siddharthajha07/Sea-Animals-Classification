# COMP 6771 - Sea-Animals-Classification


### Team Members
 
- **Kshitij Yerande - 40194579**
- **Siddhartha Jha - 40201472**

### Problem Statement
The goal of the project is to analyze the performance of the various machine learning approaches to solve image classification problem of classifying sea animals into 9 categories Corals, Crabs, Penguin, Sea Urchins, Seahorse, Seal, Sharks, Starfish,Turtle_Tortoise.

### Dataset
The dataset is retrieved from kaggle. 

Link: https://www.kaggle.com/datasets/vencerlanz09/sea-animals-image-dataste 

### Evaluation metrics

1. Accuracy: It is the most intuitive performance measure, and it is simply the ratio of correctly predicted observation to the total observations.
2. Precision: It is the ratio of the correctly predicted positive observations.
3. Recall: It is the ratio of correctly predicted positive observations to all observations in actual class.
4. F-score: It is the weighted average of precision and recall.

### Solution approaches

- Custom-CNN model: CNN architecture desined from scratch
- ResNet50 (Pre-trained) : Pretrained weights of ImageNet dataset used to train last layer on our dataset.
- SVM with HOG features(histogram of gradients) : HOG feature extracted and trained using SVM
- SVM with SIFT features: SIFT features extracted and trained using SVM

### Project Directory Structure

* **Sea-Animals-Classification**
	* data/archive
	* models/
	* metric/
	* Sea Animals Classification.ipynb
	
**Project Setup**

1. Install libraries:
	*  Pytorch
	* Numpy
	* matplotlib
	* Scipy
	* Scikit-learn
	* OpenCV
	* pandas
	* tqdm
	* torchviz
	* skimage
2. Download the data from the kaggle repository. Place all the classes in the following format.  
	* data
		* /archive
			* /corals
				* 1.png
			* /seahorse
				* 2.png
3. Create the empty folders as per directory structure
4. Run the notebook

### Results

| Model/Metric | Accuracy | F-Socre | Recall | Precision |
| --- | --- | --- | --- | --- |
| ResNet50(Pretrained) | 64.400 | 0.692 | 0.844 | 0.595 |
| Custom-CNN | 73.600 | 0.780 | 0.896 | 0.765 |
| SVM with HOG features | 46.333 | 0.492 | 0.595 | 0.437 |
| SVM with SIFT features | 9.667 | 0.101 | 0.120 | 0.125 |
