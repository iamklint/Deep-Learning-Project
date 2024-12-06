1.	Dataset Selection:
•	Used CIFAR-10 dataset, which has 10 classes of common objects
•	Implemented functionality to create balanced subsets (1000 images per class)
•	Classes include: planes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks

2.	Data Preprocessing:
•	Implemented robust data augmentation (random flips, rotations, affine transforms, color jitter)
•	Resized images to 224x224 for compatibility with ResNet
•	Normalized pixel values
•	Split data into training (80%) and validation (20%) sets, plus separate test set

3.	Model Selection:
•	Used ResNet-18 with transfer learning
•	Modified the final layer for 10-class classification
•	Implemented GPU support when available

4.	Training Pipeline:
•	Implemented full training loop with validation
•	Added learning rate scheduling (ReduceLROnPlateau)
•	Included model checkpointing to save best model
•	Tracked training and validation losses

5.	Evaluation:
•	Comprehensive evaluation metrics (accuracy, loss)
•	Confusion matrix generation
•	Separate test set evaluation

6.	Visualization:
•	Training/validation loss curves
•	Confusion matrix heatmap
•	Clear performance metrics output

