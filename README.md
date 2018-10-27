# ml-detection-malicious-http-requests

The purpose of this project is to use Machine Learning algorithms to detect malicious requests from a server log. 

### Why log analysis ? 
Log analysis involves large volume of data. For an administrator, it is really important to understand how to analyze the logs from a security standpoint. Reading through every line of log data manually is not feasible. The majority of your log data and log messages will be repetitive and normal, so repeatedly looking at the same things will be a waste of time and resources. That’s why effective log analysis relies on machine learning to identify anomalies. The solution is not to train humans to read logs, but to train algorithms to do so. 

## How will we do it ?
The obvious first step in a web log project is the preparation of data.
  *Filter and retain certain actions.
  *Identify (or split) dates and make use of them (differences between two dates etc.).
  *Clean missing or abnormal data.
  *Geographically locate the IP address.
  *Work with certain values such as the user agent of a navigator.
  *Categorize certain actions (from the URL, for example).
  *Local File Inclusion attempt.

## Steps
  *First, by using regular expressions to match all the field and for identifying different attacks present on a web application.
  *Second,
