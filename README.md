# Common-Leaf-Disease-Classification-CNN
A CNN model training script for classification of common leaf disease images that are found on common crop plants. Trained on the https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset image dataset
The .ipynb is the full training script, the .pth is the weighted state of the model, which can be loaded. 

Run Instructions -

For using built model weights:

1. Ensure pytorch, torchvision, etc. are installed

2. Create a model class in a python script to load the model file (leaf_disease_model.pth) into.
   * you can copy the model class (LeafCNN) from the LeafClassificationCNN.ipynb file in cell 6

3. Use torch.load() to read the .pth file:
 
* EG: 	model = torch.load('entire_model.pth')
 	state_dict = torch.load('leaf_disease_model.pth", weights_only=True)
	model.load_state_dict(state_dict)
	model.eval()

For Using Training script and creating new model:

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

