# USING ANSIBLE TO DEPLOY HADOOP AND SPARK WORKING ENVIRONMENT

## How is Ansible useful for deploying Hadoop?
• Hadoop requires its files to be present and running on multiple machines. The process of doing the same process in multiple machines every time repetitively could be    exhausting and is error-prone.

• This is where Ansible is valuable and helps deploy Hadoop files and other applications that require their file to be deployed in multiple machines such as Apache Spark  and Apache Drill.

• Therefore, multiple YAML files have been created to instruct the machines to download the application files and edit the system file to run the application.

• There is a local virtual machine in the deployer's computer with AWX Tower (Ansible Tower) that can pull the YAML configurations from github and update the local        configurations when running in the local Ansible virtual machine.

## What do the file names mean?
• Files that contain names with Amazon are concerned with connecting with Amazon Web Services (AWS) EC2 machines. Meanwhile, the names with google are for configuring    virtual machines with the Google Cloud Platform.

• To install Apache Spark and Pyspark, the dependencies of a particular set of versions were required, which was made convenient by using Ansible. The file called pip-    installer has the exact functions required to deploy Pyspark with Machine Learning Library.

• The Hosts file has the host's and slave machines' IP addresses. This file is directly copied to the host's file in the ubuntu Machine.

## Things that can be improved
• Maintaining a proper repository with subdirectories will help reduce the confusion and give a better interpretation of what was being tried to be done.

•	Directly communicating the command line interface of AWS and GCP for the commissioning of machines would provide more automation for this process

Please find the research report here.
https://github.com/suhailshaik98/Configure-Apache-Hadoop/blob/main/Research%20Report.pdf
