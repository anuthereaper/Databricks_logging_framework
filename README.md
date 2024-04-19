# Databricks_logging_framework
A Python logging framework designed to be used in databricks based on the Python logging module

---
page_type: sample
languages:
- python
products:
- Databricks
description: "Logging framework for Databricks based on the Python logging module"
---

# Logging framework for Databricks based on the Python logging module

<!-- 
Guidelines on README format: https://review.docs.microsoft.com/help/onboard/admin/samples/concepts/readme-template?branch=master
-->

## Create a databricks instance

Create a data bricks workspace. If you already have one then skip this step.

## Clone the repo

Create a user that has enough rights to execute all the needed statement

## Execute the main_notebook notebook 

First execute the common notebook 
%run ./log_common

Then execute the following setup the logger
logger = setup_logging("DEBUG",<log_file_path>)
Input parameters : 
level -- Minimum Level of logging to logged. Defualt is INFO (OPTIONAL).
logpath -- Path to logfile (OPTIONAL)

Finally log with a message and the level of that message.
log_message("THIS IS A DEBUG","DEBUG")
log_message("THIS IS AN INFO","INFO")
log_message("THIS IS A WARNING","WARNING")
log_message("THIS IS AN ERROR","ERROR")
log_message("THIS IS A CRITICAL","CRITICAL")
