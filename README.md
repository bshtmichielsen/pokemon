# Pokemon classification with Support Vector Machines

This project is used as the **week 4** exercise in a Machine Learning course.

Project *pokemon* demonstrates the use of a support vector machine for image recognition using pokemon images. It is set up such that one can retrain it to detect other things too, instead of pokemon.

## Exercise

First run the notebook as given to see if it loads the data correctly, after that continue with the exercise below.
For this exercise you may need to refer to the sklearn documentation on [Support Vector Machines for classification](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html).

### Hyperparameter C

The constructor of the Support Vector Machine has an optional hyperparameter named C, which by default is `1.0`. Try providing a value of `0.5` for this parameter and see if this makes any difference. Then provide a value of `2.0` for this parameter and note any differences. Which of those 3 values [`1.0`, `0.5`, `2.0`] would you say gives the best results and why? Add a text cell in which you explain your reasoning.

### Hyperparameter kernel

The constructor of the Support Vector Machine has an optional hyperparameter named `kernel`, which by default is `rbf`. Look up in the sklearn documentation which other values this hyperparameter accepts. Add a text cell in which for each one of them except `precomputed` you explain in a few sentences what kind of data they would be most suitable for. After that, add a few code cells to train the model with the different hyperparameters and compare the accuracy to see if your expectation matches with reality. Where there any surprises?
 
### Moaaahhhh Pokemon

The current notebook does fairly well probably because each of the Pokemon has a different color. Go to the original source of the Pokemon images and download images for a few more Pokemon, for example another yellow one to see if the predictions for Pikachu degrade, and another green Pokemon to see if Bulbasaur gets misclassified more often, etc. Add 4 more Pokemon in total, so the number changes from 6 to 10 classes. Rerun the notebook. Add a text cell at the bottom explaining in a few sentences what you noticed in the classification report in the Evaluation section.

### Your own images

Work together with 2 or 3 other students. Each of you download about 25 images of a certain thing that you like, for example studentA downloads 25 images of a dog, studentB download 25 images of a cat, and you download 25 images of an aeroplane. Rename the `data` folder relative to this notebook to `pokemon-data` and make a new `data` folder. Put your images in there, each in a seperate folder with the name of the thing, similarly to how the pokemon were. Run this notebook. Did it work? Why yes/no? Is this model good? Discuss with your fellow students, write their names in a new text cell at the end of the notebook and write a short summary (~150 words) of your discussion and conclusions.

