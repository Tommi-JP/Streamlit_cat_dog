# Cat or Dog Classifier on Streamlit

This is a simple web application to classify images as either a cat or a dog. The application is built using Streamlit and a pre-trained TensorFlow model.

## Features

- Upload an image and get it classified as a cat or a dog.
- Displays the uploaded image along with the classification result and confidence score.

## Setup

### Prerequisites

- Python 3.12.4
- pip
- git
- [Git LFS](https://git-lfs.github.com/)

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/Tommi-JP/Streamlit_cat_dog.git
    cd Streamlit_cat_dog
    ```

2. **Install Git LFS:**

    Follow the instructions on the [Git LFS website](https://git-lfs.github.com/) to install Git LFS.

3. **Initialize Git LFS and pull the model file:**

    ```bash
    git lfs install
    git lfs pull
    ```

4. **Install the required Python packages:**

    ```bash
    pip install -r requirements.txt
    ```

### Run the Application

1. **Start the Streamlit app:**

    ```bash
    streamlit run main.py
    ```

2. **Open your browser and go to: (if not open automaticaly)**

    ```
    http://localhost:8501
    ```

## Usage

1. Upload an image (JPG, JPEG, or PNG).
2. The app will display the uploaded image.
3. The app will classify the image as either a cat or a dog and display the result along with the confidence score.

## Model

The `cat_dog.h5` file is a pre-trained TensorFlow model used for classification. It is tracked using Git LFS due to its size.

### Adding a New Model

If you want to update or add a new model, follow these steps:

1. Replace the existing `cat_dog.h5` file with your new model file.
2. Add the new model file to Git LFS:

    ```bash
    git lfs track "cat_dog.h5"
    git add cat_dog.h5
    git commit -m "Updated model file"
    git push origin main
    ```

## License

## Acknowledgements

- [Streamlit](https://www.streamlit.io/)
- [TensorFlow](https://www.tensorflow.org/)
