# Metodi e strumenti per l'analisi della comunicazione

## Speaker info
This course is held by Andrea Giussani, Academic Fellow in Computer Science at Bocconi University.
You can reach him out either at [:email:](andrea.giussani@unibocconi.it) or on Linkedin [:zap:](https://it.linkedin.com/in/andrea-giussani)

## Repository Structure
You will find:
 - a `class_material` folder containing the class material used in this course;
 - a `extra_material` folder containing extra material from which you might benefit from;

## Setting Up the Google Colab Environment

The Google Colab is a product from Google Research which allows
> anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs.

For more information, please visit the following [link](https://research.google.com/colaboratory/faq.html).

Here, we provide a short tutorial on how to upload the data on that environemnt via Google drive, and then use the Google colab to run your analysis.
Please, note that we assume you have a google account to access to this Google product.

### 1. Open a Google Colab session

From your favourite browser, open a new colab notebook via the following [link](https://colab.research.google.com)

### 2. Mount your drive on colab

We assume you have placed the data into the `My Drive` folder. If so, connecting your drive to a google machine is pretty easy, using the python google library: just run the following code snippet

```python
from google.colab import drive
drive.mount('/content/drive')
```
After an authorisation check, you will be able to interact with your drive content either from the file browser side panel (easier) or using command-line utilities.

### 3. Clone the GitHub Repository on your Drive
I suggest to create a folder inside your drive. For example, call it `iulm-2023`. Then, in any colab notebook cell, type the following commands
```python
%cd '/content/drive/My Drive/iulm-2023'
```
and then clone the following repository:
```python
!git clone https://github.com/cloudacademy/2023-python-iulm.git
```

### 4. Open the template .ipynb file from your drive
Now, you have to navigate inside the Google Drive folder where the repo has been cloned. Once there, you just need to open, say, a ipynb file with Google Colab. And that's it! :smile:

### 5. Let's get our hands dirty
Just run the following snippet to put the raw data into a `pandas` dataframe:
```python
import pandas as pd
df = pd.read_csv('/content/drive/My Drive/<PATH_TO_FILE>/<FILENAME>.csv')
```
Are you ready? Let us get started!
