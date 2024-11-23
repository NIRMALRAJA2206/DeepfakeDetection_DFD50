# DeepfakeDetection_DFD50

Deepfake detection using deep learning: Our hybrid model DFD50 (ResNeXt-50 CNN + LSTM) effectively detects deepfakes in videos, achieving 98.91% training accuracy, 89% validation accuracy, and 96% test accuracy on combined Deepfake Detection Challenge and FaceForensics++ datasets.

## Dataset
The datasets used are listed below:
- [**FaceForensics++**](https://github.com/ondyari/FaceForensics)
- [**Deepfake Detection Challenge**](https://www.kaggle.com/c/deepfake-detection-challenge/data)

## Replicating Our Work

### Step 1: Prepare Dataset for Training
- Check the **Preprocessing.ipynb** notebook.
- Provide the paths to the video files from the FaceForensics++ and Deepfake Detection Challenge datasets.
- To see how the preprocessing works:
  Use the sample dataset:
  - Before Processing : **[SampleData](https://drive.google.com/drive/folders/1AvLHGJEZb40MOHQS7wRoVzxcCv5xucA3?usp=sharing)**
  - After Processing : **[SampleDataProcessed](https://drive.google.com/drive/folders/11j4QbYdJdiFQbAFyehcozhzMVkYhznSK?usp=sharing)**
  - To see the final preprocessed dataset, check the following drive links:
    1. [**Processed_FaceForensics++_REAL&FAKE**](https://drive.google.com/drive/folders/1flwgNo5hbL9--EuG5S8aWIjaWg2642Oj?usp=sharing)
    2. [**Processed_DeepfakeDetectionChallenge_REAL**](https://drive.google.com/drive/folders/19XSqiX39OcQImcFWNIMI6EcI3YX0Shq7?usp=sharing)
    3. [**Processed_DeepfakeDetectionChallenge_FAKE**](https://drive.google.com/drive/folders/1zXCDSigR_wI_0TYI6_5-OVDiOJPpLrnH?usp=sharing)
  
  These datasets include a total of 5,282 face-cropped videos along with a metadata.csv file that provides labels (REAL or FAKE) for each video.

### Step 2: Model Training
- Check the **ModelTrain.ipynb** notebook.
- Use the preprocessed face-cropped dataset to train the model.
    - To see the final preprocessed dataset, check the following drive links:
    1. [**Processed_FaceForensics++_REAL&FAKE**](https://drive.google.com/drive/folders/1flwgNo5hbL9--EuG5S8aWIjaWg2642Oj?usp=sharing)
    2. [**Processed_DeepfakeDetectionChallenge_REAL**](https://drive.google.com/drive/folders/19XSqiX39OcQImcFWNIMI6EcI3YX0Shq7?usp=sharing)
    3. [**Processed_DeepfakeDetectionChallenge_FAKE**](https://drive.google.com/drive/folders/1zXCDSigR_wI_0TYI6_5-OVDiOJPpLrnH?usp=sharing)

### Step 3: Model Evaluation
- Check the **predictfinal.ipynb** notebook.
- For evaluation, update the folder with the facecroped dataset for testing.
- Use this [**Preprocessed dataset for Testing**](https://drive.google.com/drive/folders/11j4QbYdJdiFQbAFyehcozhzMVkYhznSK?usp=sharing) to randomly select 150 videos and evaluate.

## Model Access
- Our Model - [**DFD50 Model**](https://drive.google.com/file/d/1mWW1Egz3jxWWL674vkljp6Y6aPQBtPG2/view?usp=sharing)
- State of art model used for comparison [**Xception Model**](https://drive.google.com/file/d/18BtAOc1IX8flm8AZ7QCxgTSOWe0EfpXJ/view?usp=sharing)

