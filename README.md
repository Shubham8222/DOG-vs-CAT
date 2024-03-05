# Cat-vs-Dog Image Classification

This project aims to classify images as either cats or dogs using machine learning techniques.

## Dataset

- **Filename**: The name of the image file.
- **Label**: The class label of the image (Cat or Dog).
- **File Type**: The file format of the image.
- **Resolution**: The dimensions of the image in pixels.
- **Notes**: Any additional notes or comments about the image.



## Requirements

- Python 3.7 or higher
- TensorFlow 2.5.0
- NumPy 1.21.0
- Jupyter Notebook (optional, for running notebooks)


## Usage

### Downloading the Dataset

To use this dataset, you can download it from [link to dataset location]. Once downloaded, extract the files to your desired location on your local machine.


An example- load images using TensorFlow:

```python
import tensorflow as tk

# Define data loading parameters
image_dir = 'path/to/dataset/images'
batch_size = 32
image_size = (224, 224)


# Load training dataset
train_generator = datagen.flow_from_directory(
    image_dir,
    target_size=image_size,
    batch_size=batch_size,
    class_mode='binary',
    subset='training'
)

# Load validation dataset
validation_generator = datagen.flow_from_directory(
    image_dir,
    target_size=image_size,
    batch_size=batch_size,
    class_mode='binary',
    subset='validation'
)

# Now you can use train_generator and validation_generator as input to your model
```


## Credits
Dataset from [Kaggle Dataset](https://www.kaggle.com/datasets/salader/dogs-vs-cats).

