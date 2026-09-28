# Star Type Classifier
A PyTorch neural network that classifies stars based on numerical data about their physical properties.

Overview
-
Model uses four features:
- temperature
- luminosity
- radius
- absolute magnitude

The project covers the full machine learning workflow, including data preprocessing, training, validation, testing, and making predictions on new star data.

Machine Learning Model
-
The classifier is a fully connected neural network built using PyTorch.

Architectures is input layer --> 64 neurons + ReLU --> 32 neurons + ReLU --> 6 output classes

The model is trained using:
- Loss function: Cross Entropy Loss
- Optimizer: Adam
- Learning rate: 0.001
- Batch size: 20
- Maximum epochs: 20
- Early stopping patience: 5 epochs

The input features are standardized using StandardScaler before being passed to the neural network.

Star Classes
-
Class --> Star Type
0 --> Red Dwarf
1 --> Brown Dwarf
2 --> White Dwarf
3 --> Main Sequence
4 --> Super Giant
5 --> Hyper Giant

Dataset
-
The project uses the Star Type Classification dataset by brsdincer on Kaggle.

Dataset: Kaggle - Star Type Classification (https://www.kaggle.com/datasets/brsdincer/star-type-classification/data)

The original dataset contains information about stars including temperature, luminosity, radius, absolute magnitude, color, and spectral class.

For this project, I used the numerical features Temperature, Luminosity, Radius, and Absolute Magnitude as inputs to the neural network.

The dataset is provided under the Database Contents License (DbCL), with the database subject to the Open Database License (ODbL). The original dataset and its licensing terms are attributed to the original creator.

Try New Star Data
-
Notebook includes a section where you can enter the properties of a star (temperature, luminosity, radius, absolute magnitude).

The trained neural network then predicts which star type the input most closely corresponds to.

Project Structure
-
star-type-classification/
├── data/
│   └── Stars.csv
├── star_type_classification.ipynb
├── requirements.txt
├── README.md
└── .gitignore

Technologies
-
- Python
- NumPy
- Pandas
- Scikit-learn
- PyTorch
- Matplotlib
- Google CoLab

Attribution
-
Dataset: Star Type Classification by brsdincer, Kaggle.

The dataset is subject to the licensing terms provided by the original dataset creator, including the Database Contents License (DbCL) and applicable Open Database License (ODbL) terms.
