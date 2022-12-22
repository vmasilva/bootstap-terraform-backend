# bootstap-terraform-backend
This script helps on the terraform initialization, creating the pre-required resources for the backend, and preparing the setup file

## The "chicken or the egg" problem

Following the best practices, the terraform backend state file should be stored in a remote secure location, which in most cases, results in using a object storage in the Cloud Provider.   

Ideally all the resources should be defined as a code, in the terraform project, however the backend storage has to be created, and, terraform also has to be initialized before that any resource could be deployed by Terraform, it's like the "chicken or the egg" problem, so, it's necessary an alternative way to create the pre-required resources.  
