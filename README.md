Anura Deshpande

anurades@usc.edu

Completed at the end of my curriculum experience in USC's CAIS++, I developed a convolutional neural network (CNN) to classify seven emotions based on images of human facial expressions.

The dataset utilized was Kaggle's "FER 2013," which contains 28,709 training images and 3,589 test images, each being 48x48-pixel grayscale images depicting centered facial emotions across seven categories: angry, disgust, fear, happy, sad, surprise, and neutral. To prepare the dataset for a computer vision task, I rescaled pixel values by dividing them by 255, ensured uniform dimensions and color scales, converted class labels (0–6) into one-hot encoded vectors, and set the batch size to 64. These preprocessing steps ensured standardization across the images and established a basis for efficient computation.

I implemented a CNN due to its effectiveness in feature extraction and image classification tasks. The architecture consisted of three convolutional layers with filter sizes of 64, 128, and 256, kernel sizes of 3x3, and ReLU activation functions to capture non-linearities. This was followed by three max pooling layers of size 2x2 to reduce computational complexity, one flatten layer, and two dense layers, with the final layer comprising seven output classes and a softmax activation function. The model was trained using categorical cross-entropy loss, suitable for multiclass classification with one-hot encoding, and the Adam optimizer for its dynamic learning rate. Training was conducted over 20 epochs to minimize the risk of overfitting.

The test accurcacy of the model was 0.57. The highest precision value was 0.24, while the highest recall was 0.25, both for the happy classification.

The current dataset, model architecture, training procedures, and metrics are not fully optimized for robust emotion recognition and leave much room for improvement. The chosen CNN architecture is likely too simple and does not capture the intricate patterns required for distinguishing subtle nuances in between facial expressions. 

This project can have significantly wider implications, such as enabling real-time facial expression recognition in interactive systems, including chatbots, robotics, and virtual assistants, which could enhance user experiences across industries like education, healthcare, and customer service. However, these applications come with limitations and ethical concerns. Facial scanning raises privacy issues, and implementing such systems requires adherence to data protection regulations and obtaining explicit user consent. Additionally, the dataset must remain current and culturally representative to avoid bias in predictions, as facial expressions and their interpretations can vary across demographics, suggesting the need for a larger and more diverse dataset than the implemented FER 2013.

If I were to continue this project, I would focus on improving the model's performance by refining its architecture and incorporating transfer learning with a pre-trained model like ResNet. Finally, to further improve the system's capabilities, I would expand the identifiable emotional classifications and train the model on a larger dataset.


