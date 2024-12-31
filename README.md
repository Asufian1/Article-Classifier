One of the projects I worked on involved building a Naive Bayes classifier to distinguish between articles from two magazines: 
The Economist and The Onion. The Economist publishes serious articles, while The Onion is more satirical, so the goal was to train 
a model to classify which article came from which magazine.

We were given a dataset of text articles that had already been pre-processed into feature vectors. Each vector represented whether 
certain words appeared in an article, and the labels indicated the magazine it came from. Using the Naive Bayes algorithm, I trained the 
model to predict the most probable magazine based on the words in the article.

For this project, I used Python libraries like NumPy to efficiently manipulate and process the data. For example, I used NumPy to compute 
probabilities in log-space, which helps prevent numerical precision issues when dealing with very small probabilities. I also used it to sum
log probabilities and compare values to make predictions for each test article.

I wrote Python functions to calculate probabilities, estimate parameters for the words and classes, and classify new articles. I also used SciPy
to load the dataset, which was provided in MATLAB format. Once the data was loaded and converted into arrays, I used NumPy to perform operations like
summing probabilities and calculating the maximum likelihood for each class.

By training and testing the model on datasets of different sizes, I observed how having more or less data affects performance. For instance, 
with smaller training data, the prior assumptions of the model became more influential. Additionally, I analyzed which words were most likely 
to appear in each class and which words were best at distinguishing between the two magazines, helping me understand the underlying patterns in the data.
