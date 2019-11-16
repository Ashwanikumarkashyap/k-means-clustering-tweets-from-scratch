# KNN - Tweets Clustering

The project includes implementation of K-nearest neighbour algorithm (an unsupervised learning algorithm) without using any libraries. The Objective of this project is to cluster the simmilar tweets based on similarity of words within the sentences. At the end of each experiment for different values of k, sum of squared error (SEE) is computed. The algorithm uses Jaccard distance to compute the numerical distances betweeen two tweets "http://en.wikipedia.org/wiki/Jaccard_index". Dynamic programming is also utilizied within the code in order to improve the computational running time of the program.

## Sample Output from the twitter dataset

* Dataset URL : https://archive.ics.uci.edu/ml/datasets/Health+News+in+Twitter

* K = 3
    * SSE = 3462.671
        * cluster 1: 1511 tweets
        * cluster 2: 809 tweets
        * cluster 3: 1609 tweets

* K = 5 
    * SSE = 335.843
        * cluster 1:  1526 tweets
        * cluster 2:  579 tweets 
        * cluster 3:  720 tweets 
        * cluster 4:  758 tweets 
        * cluster 5:  346 tweets 

## Programming Instructions

1) If the system don't have python Installed in it, first install python (version greater than or equal v3.7)
	- https://www.python.org/downloads/
2) The code uses the following python native libraries
        - random
	- re
	- math
3) In the root directory of the project, execute the given command from command line:
	- "python main.py"

4) Output from a sample run is also stored in a file named "output.txt" for the reference.

Notes :
 a) The code uses "bbchealth.txt" by default for the tweets data.
	- A user can change the url path to another data file as desired from the given files.

 b) The code uses, "3 clusters" by default and performs "5 experiments" one after another.
	- Each experiment increases the number of clusters being used from the previous experiment by 1.
	- A user can change the default value of intial clusters (k) and number of experiments to be performed.

 c) The program returns the value of SSE (sum of squared error) and size of each cluster after every experiment.

 d) A user can also print tweets in each cluster by uncommenting certain part of code written in the __main__.
