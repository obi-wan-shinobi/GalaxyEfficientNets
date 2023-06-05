# GalaxyEfficientNets

We present the state of the art EfficientNets being used for Galaxy Morphology Classification. 

The directories contain models used for regression or classification. The [Other Networks](Other%20Networks) directory contains the classification problem attempted using other state of the art networks.

The dataset for the regression model can be downloaded [here](https://www.kaggle.com/c/galaxy-zoo-the-galaxy-challenge).

The dataset for the classification model can be downloaded [here](http://www.mediafire.com/file/5vy5gcn5phkg6cw/GalaxyClassification.zip/file).

For more information, refer [Galaxy Morphology Classification using EfficientNet Architectures](https://github.com/obi-wan-shinobi/galaxy-morphology-paper/blob/master/Main_Paper.pdf)

# Goals and objectives

Studying galaxies and classifying them into different classes is a long-standing problem. Physicists have been trying to identify and segregate galaxies into individual groups and study their traits to understand the formation of these galaxies and relating the physics that creates them. Morphology is determined by the physical characteristics and the orbital structure of the galaxies. The shape of the galaxy potentials determines which orbital families are present. Stars moving in the specific parts of the space phase generate morphological features such as bars, rings, peanut bulges, pseudo-bulges, etc.

The main goal of the project was to study and develop a sound system for automatic classification of galaxies into these different morphological classes.

# The problem

Visual classification of galaxies into morphological classes is a tiresome process and requires a significant amount of man-power. With the advent of sky surveys, the amount of information that is gathered has increased exponentially and the need for an automated system that classifies galaxies by extracting its morphological features became even more noticeable. To implement such system, we decided to use the power of deep learning to our advantage.

The project focused mainly on two problems i.e. a regression problem which involved calculating the vote-fractions of morphological features for a galaxy using CNNs and a classification problem where we eliminate the need for these vote fraction predictions and directly classify the given galaxy image into one of the 7 classes categorized by these vote fractions in the triaining data.

We explored the usage of ensemble of EfficientNet architectures and achieved decent results with the vote-fraction predictions. The classification model achieved sound results with classification task and we successfully implemented a system that classifies given galaxy into its respective morphology

# Results

We achieved really decent results with the EfficientNet models but we decided to use an ensemble of more than one model to achieve a greater score so as to grab a place on the public leaderboard of the Galaxy Zoo 2 challenge. 

Our results were graded using the standard competition metric, i.e. the rmse score. We achieved an rmse score of 0.07765 and ranked in the top 3 on the public leaderboard.

The classification model provided us with decent accuracy of 93.7% on classifying the galaxies into 7 classes with an F1 score of 0.8857.
