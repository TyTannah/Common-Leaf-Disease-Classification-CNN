# Common-Leaf-Disease-Classification-CNN
A CNN model training script for classification of common leaf disease images that are found on common crop plants. Trained on the https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset image dataset
The .ipynb is the full script used for training. 

Run Instructions -

1. Open notebook file ide of choice (eg jupyter notebook/lab)

2. Download dataset as zip from https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset

3. Unzip contents to same folder as the notebook file. Ensure in that the unzipped folder that is created
   is called PlantVillage and that it contains folders of different plants and diseases. EG Tomato_early_blight.
   Make sure that there isn't a second PlantVillage folder within the original PlantVillage folder or issues
   may arise.

4. Pip install any libraries that are missing requirements from:
   pytorch, torchvision, numpy, matplotlib, sklearn

5. Run the notebook file

*Recommended to make sure you have the cuda version of pytorch with gpu enabled for faster execution time.

