# Style Guide for MagicSchoolBus

In anticipation of the many Jupyter notebooks and Python scripts other resources we will use for this project, 
I hope we can generate a style guide of sorts to help keep the storage of files and links consistent and accessible.
I believe that having consistency in the various aspects of our repo will also make it much easier for people to appreciate the work we have done for this hackathon.
Feel free to change or add anything you think would be a good practice for us!

## Coding
If code is copied/referenced from elsewhere, attribution should be given. 
At the same time, the code should be refactored (the coding version of paraphrasing) when possible.

**Format for attribution:**

```
import pandas as pd

df = pd.read_csv('textfile.txt')

## Attribution as comment prior to code
# Evan: https://website.com/page
newdf = df[1]
print(newdf.shape())
# arigato
## Close off with arigato because we aren't savages

```

## Jupyter Notebooks
* Save in folder `Notebooks`
* Name the notebook according to the function of the notebook using CamelCase ie. `ProductTitleClassification.ipynb`

## Python Scripts
* Goes in folder `PythonScripts`
* Name the script according to the function of the script using CamelCase ie. `Word2Vec.py`

## Links/References
* Include in `Canonicals.md`.
* Include short description of link so that it's easier to come back to in future

## Weights
* Weights generated from checkpoints for the `TitleClass` model should be stored in `Weights/TitleClass`
* Weights generated from checkpoints for the `ImageClass` model should be stored in `Weights/ImageClass`
* In the event that the two models are merged, the subfolders will be depreciated 
(unless it is seen to be advantageous to keep the individual model weights) and model weights will be stored in `Weights`
* Checkpoint Weights should be named as following: `[ModelName]_[ddmmyy,DayStartedTraining]_[4DigitCheckpointoftheDay].h5`
* Example: `TitleClass_040319_0021.h5`
* This format will be subject to change, an alternative to consider is simply `[ModelName]_[ddmmyy]_[accuracy].h5`

