## Report on the Neural Network Model

# 1)	Overview of the analysis

The purpose of the analysis is to develop a tool that will help the non-profit foundation Alphabet Soup select applicants for funding. With knowledge of machine learning and neural networks, use the features in the dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

To do this Alphabet Soup have provided a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Focussing on the following columns containing the metadata will help to create the model.

•	EIN and NAME—Identification columns

•	APPLICATION_TYPE—Alphabet Soup application type

•	AFFILIATION—Affiliated sector of industry

•	CLASSIFICATION—Government organization classification

•	USE_CASE—Use case for funding

•	ORGANIZATION—Organization type

•	STATUS—Active status

•	INCOME_AMT—Income classification

•	SPECIAL_CONSIDERATIONS—Special considerations for application

•	ASK_AMT—Funding amount requested

•	IS_SUCCESSFUL—Was the money used effectively

Note: This model and code are run within Google Colab.

# 2)	Results

**•	Data Pre-processing**

o	The target variables for the model focus on the above columns minus EIN and NAME. These are considered non-beneficial and are neither targets or features.

o	The following columns are looked at for binning. APPLICATION_TYPE, CLASSIFICATION.

o	Categorical data is converted to numeric after looking at data types.

o	Processed data is split into our features and target arrays. Into training and testing dataset.

o	Scale the data using StandardScalar

**•	Compiling, Training, and Evaluating the Model**

Using two hidden layers with 80 and 30 neurons to compile the model. After 100 epochs the accuracy increased from a loss of 0.5544 to 0.7282. 
What could be done to improve the accuracy is to bin further columns, increase the number of layers and neuron epochs alongside changing the activation functions.

# 3)	Summary
Through multiple iterations a model was initially created that did not achieve an accuracy of more that 0.7282. With more testing and time by removing and binning columns a higher score of accuracy could be achieved. If this results in a much-improved score, then the model is successful if there is only a small increase then the model may not be as successful.
