# Cat-Or-Dog
Image Classification with SVM and H.O.G.
---
As humans, it's easy to identify differences between two subjects. How does a machine tell them apart? One such way is through Support Vector Machines (SVM), a supervised learning model that analyzes data used for classification and regression tasks. 

In this project, you'll learn to train SVM for classifying images of cats and dogs by extracting Histogram of Oriented Gradients (H.O.G.) features from the input. Notably, we can use the model on any new image that we upload!

## **Table of Contents**

<ol>
    <li><a href="https://#Objectives">Objectives</a></li>
    <li>
        <a href="https://#Setup">Setup</a>
        <ol>
            <li><a href="https://#Installing-Required-Libraries">Installing Required Libraries</a></li>
            <li><a href="https://#Importing-Required-Libraries">Importing Required Libraries</a></li>
            <li><a href="https://#Defining-Helper-Functions">Defining Helper Functions</a></li>
        </ol>
    </li>
    <li>
       <a href="https://#Download-Image-Annotations">Download Image Annotations</a>
    </li>
    <li>
       <a href="https://#Histogram-of-Oriented-Gradients-(H.O.G.)">Histogram of Oriented Gradients (H.O.G.)</a>
    </li>
    <li>
       <a href="https://#Load-Images-into-Train/Test-Sets">Load Images into Train/Test Sets</a>
    </li>
    <li>
       <a href="https://#Hyperparameter-Tuning">Hyperparameter Tuning</a>
    </li>
    <li>
       <a href="https://#Predict-New-Images">Predict New Images</a>
    </li>
</ol>


## Objectives

After completing this guided project you will be able to:

*   Extract H.O.G. features from images
*   Train an SVM model on image inputs
*   Tune hyperparameters with Grid Search and evaluate model performance
*   Classify new images of cats and dogs with SVM


## Setup
For this guided project, we will be using the following libraries:

*   [`numpy`](https://numpy.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for mathematical operations.
*   [`OpenCV`](https://docs.opencv.org/4.x/index.html?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for other image processing functions.
*   [`scikit-learn`](https://scikit-learn.org/stable/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for machine learning and machine-learning-pipeline related functions.
*   [`matplotlib`](https://matplotlib.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for additional plotting tools.


### Installing Required Libraries

The following required libraries are pre-installed in the Skills Network Labs environment. However, if you run this notebook commands in a different Jupyter environment (e.g. Watson Studio or Ananconda), you will need to install these libraries by removing the `#` sign before `!mamba` in the code cell below.
