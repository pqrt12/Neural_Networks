# Neural_Networks
# Challenge
This Challenge builds neural network models to predict whether an Alphabet Soup charity funding would be successful. All work is presented in [AlphabetSoupChallenge.ipynb](https://github.com/pqrt12/Neural_Networks/blob/master/AlphabetSoupChallenge.ipynb).

Almost all of the models would yield a predictive accuracy higher than 72.5%, while to the training set data, the accuracy reaches around 73.5%. This indicates our models are not suffering from over-fit; and more layers, more neural nodes, or more epoches do not further improve the accuracy with this processed dataset.

The final model of this Challenge is saved in "one_layers.h5". It is chosen because it is simpler and with similar accuracy 72.71%. It has one hidden layer with 20 neural nodes. 

Tring to get a higher accuracy, most work is done in data preprocessing. The categorical variables are gathered in a table with their occurrence count and the "IS_SUCCESSFUL" rate. When bucketing, the infrequent values are grouped into two categories based on their "IS_SUCCESSFUL" rate. 

Columns "STATUS" and "SPECIAL_CONSIDERATIONS" are both binary variables, with one value being very rare. And their "IS_SUCCESSFUL" rates are similar.They are both dropped.

The Column "ASK_AMT" numbers span a wide range. A logarithm is performed on this column.

All of these efforts should be helpful in general, but they do not change the accuracy meaningfully to this dataset.  

Four neural network models are presented in the jupyter Notebook. There are two One-Layer networks (30 nodes vs 20 nodes), a Two-Layer network, and a Three-layer network. They are all performed similarly.

With this data preprocessing, or with the final processed dataset, the supervised learning (classification) would achieve a similar result. And there we could see the significance among the input features, and possibly cut off insignificant features to improve the accuracy.
