# deep-learning-challenge
All of the code was written independently and with the help of the Xpert AI tool. It can be found in Starter_Code.ipynb in the deep-learning-challenge repository.

REPORT:

1) Overview of analysis:
The purpose of this analysis is to utilize the tools of machine learning to make some predictions about the projects of the applicants to determine whose will be successful. This, in turn, will help the employers choose the correct applicants. Informed decisions can be made based on evidence and not anecdote. This allows for the distribution of limited resources to be as minimally wasteful as possible.

2.1) The target variable is "is_successful" as it informs us who has been successful in the past and will be used to determine. The target features are every other column as it adds a layer of analysis except "ein" and "name" which should be removed. This was done using the drop feature. Data was further pre-processed by setting a limit to the value counts of "classification" and "application_type". Finally, pd.get_dummies was used to render data numerical and thus usable.

2.2) two hidden layers - first one has 80 neurons and second one has 40, resulting in 6,161 trainable layers (and 0 untrainable). The model was then trained with 80 epochs resulting in an accuracy of 0.7210.

3) To summarize, the accuracy of this model attempting to predict which applicants to choose is 0.72 with a loss of 0.58. Perhaps, training with more epochs could refine the algorithm further.