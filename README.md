# deep-learning-challenge

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
	IS_SUCCESSFUL Column
What variable(s) are the features for your model?
	All columns except IS_SUCCESSFULnwhich is our target
What variable(s) should be removed from the input data because they are neither targets nor features?
	Columns dropped were EIN and NAME
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
    
    This is Attempt #1
    APPLICATION_TYPE cutoff = 600
    CLASSIFICATION cutoff = 300
    layer1 = 9 : activation function = relu
    layer2 = 18 : activation function = relu

    Loss: 0.5540710687637329, Accuracy: 0.7259474992752075

    A loss value of 55 indicates that the model can be further optimized.
    The accuracy percent shows that 72% of the model's predicted values align with the true values in the original dataset.

    This is Attempt #2
    APPLICATION_TYPE cutoff = 600
    CLASSIFICATION cutoff = 300
    layer1 = 9 : activation function = relu
    layer2 = 18 : activation function = relu
    layer3 = 27 : activation function = relu

    Loss: 0.5538796186447144, Accuracy: 0.7318950295448303

    A loss value of 55 indicates that the model can be further optimized.
    The accuracy percent shows that 73% of the model's predicted values align with the true values in the original dataset.

    This is Attempt #3
    APPLICATION_TYPE cutoff = 600
    CLASSIFICATION cutoff = 300
    layer1 = 80 : activation function = relu
    layer2 = 30 : activation function = tanh
    layer3 = 30 : activation function = tanh

    Loss: 0.5590451955795288, Accuracy: 0.7229154706001282

    A loss value of 55 indicates that the model can be further optimized.
    The accuracy percent shows that 72% of the model's predicted values align with the true values in the original dataset.

Were you able to achieve the target model performance?

	In the three attempts I made, the model was unable to achieve a target predictive accuracy higher than 73.1%.

What steps did you take in your attempts to increase model performance?

	I tried increasing the number of hidden layers, the number of neurons and finally different activation functions. All of which
    resulted in little to no improvement

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

	I would consider using another classification model to see if it is better at predicting whether applicants will be successful 
    	if  funded by Alphabet Soup.
