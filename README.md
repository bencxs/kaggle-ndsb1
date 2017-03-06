# kaggle-ndsb1
Kaggle National Data Science Bowl Competition - Plankton Classification

![Image of Planktons](https://kaggle2.blob.core.windows.net/competitions/kaggle/3978/media/plankton%20schmorgasborg.jpg)

[Image source](https://www.kaggle.com/c/datasciencebowl/data)

## Introduction
Implementation of the 2015 National Data Science Bowl Competition using deep neural networks.

For further information, please see the [link to the competition in Kaggle](https://www.kaggle.com/c/datasciencebowl).

Dataset can be downloaded at [Kaggle's data page](https://www.kaggle.com/c/datasciencebowl/data).

## Libraries / Packages
* TensorFlow
* TFLearn
* Python
* sklearn
* numpy
* OpenCV

## How to Use
- Download the [train.zip](https://www.kaggle.com/c/datasciencebowl/download/train.zip) and [test.zip](https://www.kaggle.com/c/datasciencebowl/download/test.zip) dataset files and place them in a folder called 'data' in your working directory.

- Open `model.ipynb` and change the `main_dir` to your directory containing the zipped files and `aug_dir` to your desired image augmented save path.

Example:
```
main_dir = 'C:/User/ABC/workingdir/data'

aug_dir = 'C:/User/ABC/workingdir/data/aug'
```

- Run the first code block in `model.ipynb` to extract the zip files. You will see that the zip files are extracted in the following folder structure:

```
workingdir
    ---data
        ---train
            ---acantharia_protist
                ---001.jpg
        ---test
            ---xxx
                ---xxx.jpg
```

- Run the remaining code blocks to complete the image preprocessing and model training.

## Status
* Base Inception V3 model implemented
* [WIP] To experiment on other model architectures
