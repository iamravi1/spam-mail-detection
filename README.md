# Spam-mail-detectionπ¨
> A Deep learning model to identify the spam mail using BERT pre trained model.
## The Pipeline Overview for Spam Detection Using BERT
To build the system ourselves we are going to follow these procedures:

1. Load Data β We will be loading our data which is simple [2 categories(ham and spam) along with corresponding emails] CSV file. The file can be found here

2. EDA β Perform some EDA to get a feel of what data looks like β statistics here!

3. Pre Processing β Based on the results of EDA we will be going to apply some preprocessing to the data to make it model friendly

4. Model Creation β We will use Functional API* to build our Deep Learning Model which will consist of

- INPUT β Will create an input layer that will take in all the pre-processing data and pass it to bert_processor.
- BERT PREPROCESSOR β Process our input text to be in the format which encoder accepts. (adds MASK AND ENCODINGS).
- BERT ENCODER β Feed our processed text to the bert model which will eventually generate a contextualized word embedding for our training data.
- DROPOUT β Add a dropout layer that will randomly drop out a few neurons from the network to take care overfitting problem.
- SOFTMAX β At last we will add a softmax layer to predict data in 2 categories.

5. Model Evaluation β Further we will check how the model performs on the test data and plot some relevant charts and metrics based on the observations.

6. Predict Data β Finally we will predict our own emails using the model.  

<img src="https://editor.analyticsvidhya.com/uploads/91446MODEL%20PIPELINE.PNG" style="height: 450px; width:1050px;"/>
