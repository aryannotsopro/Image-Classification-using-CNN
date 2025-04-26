# Image-Classification-using-CNN
The Image Classification using CNN project aimed to develop a deep learning model capable of accurately classifying images from the CIFAR-10 dataset, which contains 60,000 32x32 color images across 10 distinct classes (such as airplanes, cats, cars, and ships).

The project started with data preprocessing, which involved normalizing pixel values to a 0–1 range and applying data augmentation techniques like rotation, flipping, zooming, and shifting. This helped prevent overfitting and improved the model's ability to generalize on unseen data. Additionally, class balancing techniques were applied to handle any potential imbalance in the dataset.

The CNN architecture was carefully designed with multiple layers:

Convolutional layers to extract spatial features,

Pooling layers (like MaxPooling) to reduce dimensionality and computation,

Dropout layers to prevent overfitting,

Fully connected dense layers to map the extracted features to output classes.

The model was trained using the Adam optimizer for faster convergence, and techniques like early stopping and learning rate reduction were used to fine-tune performance and prevent overtraining.

After training, model interpretability was a key focus. To make the model's decisions more transparent, Grad-CAM (Gradient-weighted Class Activation Mapping) was implemented. Grad-CAM allowed visualization of the important regions in the input image that the CNN focused on while making its predictions, giving insights into the model's decision-making process.

Finally, the model was tested on unseen images to validate its generalization capability, achieving reliable accuracy and producing real-time predictions by integrating the trained model into a prediction pipeline.
