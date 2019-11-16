1) If the system don't have python Installed in it, first install python (version greater than or equal v3.7)
	- https://www.python.org/downloads/
2) The code uses the following python native libraries
        - random
	- re
	- math
3) In the root directory of the project, execute the given command from command line:
	- "python main.py"

Notes :
 a) The code uses "nprhealth.txt" by default for the tweets data.
	- A user can change the url path to another data file as desired from the given files.

 b) The code uses, "3 clusters" by default and performs "5 experiments" one after another.
	- Each experiment increases the number of clusters being used from the previous experiment by 1.
	- A user can change the default value of intial clusters (k) and number of experiments to be performed.

 c) The program returns the value of SSE (sum of squared error) and size of each cluster after every experiment.

 d) A user can also print tweets in each cluster by uncommenting certain part of code written in the __main__.