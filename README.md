# Implementation of the soft margin SVM using different gradient descent methods

Implement the SVM algorithm for all of three gradient descent techniques.
1. Batch gradient descent
2. Stochastic gradient descent
3. Mini batch gradient descent

```features.txt```Each line contains features (comma-separated values) for a single datapoint. It has 6414 datapoints (rows) and 122 features (columns).

```target.txt```Each line contains the target variable (y = -1 or 1) for the corresponding row in features.txt.

Time Taken by each techinque:
```
BGD - 0.1467 seconds 
SGD - 0.0488 seconds 
Mini BGD - 0.0448 seconds
```

Total Number of Iterations by each techinque:
```
BGD - 57
SGD - 2523
Mini BGD - 947
```

**The Graph is avaiable in SVM_Gradient.ipynb file**

The difference between all the three methods is straightforward; Batch gradient descent takes all the data and updates the beta values for every iteration. Even though it took fewer iterations to converge, it took more time to compute than the rest of the methods. Next, coming to stochastic gradient descent, we first shuffle the data, read and send only one data for updating the values. So just for one iteration, it would have updated the size of the data times. We can see that in the graph, even though it took many iterations to converge, it took 0.0488 secs. The mini-batch gradient descent is the same as stochastic gradient descent. The only difference is, we send a small batch every time instead of only one value of data. We can say that it is the best technique as it has less time and fewer iterations.
