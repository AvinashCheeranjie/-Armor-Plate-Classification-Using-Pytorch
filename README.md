# Simple CNN for Binary Classification

Project for the 2024-2025 Challenge for MacRoboMaster Computer Vision team.

The project involves training a model to perform binary image classification on a custom dataset. It classifies whether or not an armor plate is visible in a given image.

## Training the Model

To train the model on your labelled dataset, run the first 4 cells in the armor_plate_classifier.ipynb file. Ensure you set the path to your dataset when creating a ArmorPlateDataset object:

```python
folder_path = 'path/to/train/data' # Replace with path to your dataset
dataset = ArmorPlateDataset(folder_path=folder_path, transform=transform)
```
## Testing the Model

To test the model on an unseen image, call the predict() function by passing a SimpleCNN object and the path to your image:  

```python
test_image = 'path/to/test/image.png' # Replace with path to your image
print(f'Armor present: {predict(model, test_image)}') # model = SimpleCNN()
```
