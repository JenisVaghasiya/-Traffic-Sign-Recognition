Loading and Preprocessing Data: The load_data function reads images and their labels, resizing images to 32x32 pixels. Images are normalized by dividing pixel values by 255.0.

Data Augmentation: The ImageDataGenerator is used for augmenting the training data by applying random transformations such as rotation, width/height shifts, shear, and zoom.

Model Architecture: A pre-trained VGG16 model (without the top layer) is used as the base. Additional layers (Flatten, Dense, BatchNormalization, Dropout) are added on top of VGG16.

Training and Tuning: The model is compiled with the Adam optimizer and trained for 30 epochs using augmented data. The training history is stored for later visualization.

Evaluation: The model is evaluated on the test set, and the test accuracy is printed. A classification report and confusion matrix are generated to analyze performance.

Visualization: Training history is plotted to visualize accuracy and loss over epochs. The confusion matrix is also visualized using Seaborn.
