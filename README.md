### Project Title: Signs of Ageing

#### Problem Statement:
A model to classify and localize different signs of ageing such as puffy eyes, wrinkles, dark spots, etc., on the face.

#### Abstraction:
**EfficientDet: Scalable and Efficient Object Detection**  
EfficientDet is a type of object detection model, which utilizes several optimization and backbone tweaks, such as the use of a BiFPN, and a compound scaling method that uniformly scales the resolution, depth, and width for all backbones, feature networks, and box/class prediction networks at the same time. We are using the EfficientDet Object Detection model to classify and localize different signs of ageing such as puffy eyes, wrinkles, dark spots, etc., on the face. Image processing techniques are used to process the image as per requirements.

---

### Methodology to be Used

#### 1. Accumulating Dataset
- Collecting images with different features and in different environment factors.
- Annotating the images using 2 ways:
  - Automated (Ex: AWS SageMaker)
  - Manual (Ex: LabelImg, Labelme)

#### 2. Pre-processing Data
- Using Roboflow, any form of data can be loaded and processed.
- The dataset to be fed into the model will be created using Roboflow.
- Data cleaning will also be done along with creation.
- The obtained dataset can be split into training and testing.
- Pre-processing and Augmentation will be done.
- The health of the dataset will be checked i.e., Class balance, Annotation heat map.

#### 3. Building the Object Detection Model
- Clone the Tensorflow models' repository.
- Install the Object Detection API.
- Run model builder test in the GitHub repository to test the working of the models.
- Prepare Tensorflow 2 Object Detection Training Data.
  - Roboflow automatically creates our TFRecord and label_map files that we need.
- Configure Custom TensorFlow2 Object Detection Training Configuration.
- Prepare the object detection model by writing a custom configuration file:
  - Slotting our dataset, model checkpoint, and training parameters into the base pipeline file.

#### 4. Train Custom TF2 Object Detector

#### 5. TensorFlow2 Object Detector
- Download test images from Roboflow which were already made in the second phase and now test the model.

#### 6. Run Detector on a Test Image

---

This structured approach ensures that the project is methodically executed from data accumulation to model deployment and testing, ensuring clarity and coherence throughout the process.
