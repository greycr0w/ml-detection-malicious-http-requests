# ml-detection-malicious-http-requests

The purpose of this project is to use Machine Learning algorithms to detect malicious requests from a server log. 

### Why log analysis ? 
Log analysis involves large volume of data. For an administrator, it is really important to understand how to analyze the logs from a security standpoint. Reading through every line of log data manually is not feasible. The majority of your log data and log messages will be repetitive and normal, so repeatedly looking at the same things will be a waste of time and resources. That’s why effective log analysis relies on machine learning to identify anomalies. The solution is not to train humans to read logs, but to train algorithms to do so. 

## How will we do it ?
#### 1. Cleaning the data
The obvious first step in a web log project is the preparation of data. By using regular expressions to match all the different fields on our data, we also use regular expressions for identifying different attacks attempts on the server.  
Here are the steps we took:
  * Make a pandas dataframe
  * Split each requests
  * Filter and retain certain actions.
  * Identify (or split) dates and make use of them (differences between two dates etc.).
  * Work with certain values such as the user agent of a navigator.
  * Categorize certain actions (from the URL, for example).
  * Look for any attack attempts on the request content request like: Local File Inclusion attempt, injections,...


#### 2. Visualize our data

To understand our data, we will try to visualize it from charts, maps, scatter plots,…
  
  
#### 3. Apply Machine Learning

From there we will choose the relevant features in detecting a hacking attempt and come up with a way to quantify these values. This will allow us to explore the dataset in many ways that give us insight into the different classes/types of request that exist. Such classes would include hackers, bots and regular users. We will then apply some clustering algorithms and analyse the results referring back to the original data to see if you can manually identify the clusters. Once we are happy with our cluster labelling, we can move on to using some supervised learning algorithms and analyse how they perform.
