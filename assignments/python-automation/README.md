# 📘 Assignment: Python Automation for Everyday Tasks

## 🎯 Objective

Learn how to automate a simple repetitive task in Python by reading data from a file, organizing it, and creating a useful summary report.

## 📝 Tasks

### 🛠️ Read and Process a List

#### Description
Write a script that opens a text file containing a list of tasks, reads each line, and turns it into a usable Python list.

#### Requirements
Completed program should:

- Open a text file named `tasks.txt`
- Read each line and remove extra whitespace
- Ignore blank lines
- Store valid entries in a list
- Print the total number of tasks found

### 🛠️ Filter and Organize Data

#### Description
Add logic to separate completed and incomplete tasks from the list.

#### Requirements
Completed program should:

- Use a simple format such as `TaskName - done` or `TaskName - pending`
- Check whether each task is complete
- Create two lists: one for completed tasks and one for remaining tasks
- Print both groups in a clear, readable format

### 🛠️ Save a Report

#### Description
Create a final report file that summarizes the task list for easy review.

#### Requirements
Completed program should:

- Write a report file named `task_report.txt`
- Include the total number of tasks, completed tasks, and remaining tasks
- List the incomplete tasks in a neat summary
- Save the report in the same folder as the script
