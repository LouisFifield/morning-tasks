# Terraform
​
1. What is infrastructure as code (IaC) and why is it important in modern IT operations? What are the advantages?

Infrastructure as code (IaC) is a method which uses code to manage and provision computer data centres as opposed to physical configurations or those done through a interactive user interface. It is very important in modern IT operations because 

IaC has many advantages over traditional methods of managing infrastructure. The first is increased consistency, as the code is the same and can be deployed at the press of a button, it can be repeated across various environments to keep the operation of the systems the same. The second advantage is that because the management of infrastructure is automated, costs are not expended in managing and maintaining the systems manually. The third advantage is speed of deployment, as infrastructure is deployed simply by changing the code, you can deploy and change the infrastructure very quickly. As the infrastructure can be seen in a code format, it can be communicated easily through the platform of GitHub and teams developers and IT professionals can collaborate producing the best systems possible.  
​
2. Explain the concept of "Infrastructure as Code" (IaC) and how Terraform fits into this concept.
​
The concept of Infra

3. What problems do modules help address, and how do they promote reusability?
​
4. Explain in your own words what the following commands achieve;
​
- `terraform init`
​
This command sets up the terraform working directory, which is the main project file where you store and organise the terraform configuration files you have created to describe the infrastructure you want to create and manage using terraform. The command instructs terraform to look at the resources in our code and then downloads the particular plugins which works with the specific provider (AWS, azure, gcp etc) and stores them locally. Terraform init also downloads the latest versions of modules you have specified in your code preparing them to be used when building the infrastructure.   

The plugins are stored in a file called .terraform/ 

- `terraform plan`

Assesses what the current state of the infrastructure, via terraform statefiles to understand the existing resources and their settings. It then reads the configuration files (.tf files with resources in them) compares this current state with the desired state to understand what needs to be modified, created or deleted and then presents an execution plan detailing the sequence of actions that Terraform will take to achieve the desired configuration of the infrastructure. It is to be noted that terraform plan only produces a plan it does not make any actual changes to the infrastructure. The plan helps one to more fully understand the changes that the code they have will implement. 

terraform state files - Is a JSON formatted file that is created when you run terraform apply. It keeps track of the current state of the infrastructure managed by terraform, storing information on the resources created. It is to be noted that this file holds the layout of your infrastructure and secret sensitive information and as such should not be shared or versioned in public repositories. 

- `terraform apply`

This command is similar to terraform plan except that it takes the process one step further and implements the changes written in the configuration files to the infrastructure you are working with. 
​
- `terraform destroy`

This command is used to delete and wipe everything from the infrastructure which is included in the configuration files. It ​Works by reading the configuration (.tf) files, validating that they have no syntax errors, then creating and presenting a destruction plan, which is to be confirmed by the user. The command then deletes the resources, updates the statefile and shows what has been destroyed. 

- `terraform fmt`

​This command formats the terraform code in the workspace to make sure that it is well organised and presented in a consistent style. 

- `terraform output`
​
This command can be used by itself or with arguments. When it is applied by itself it lists all of the output values defined in the configuration. When connected with a argument. 

terraform output instance_ip; 

this will display the value of the outpur instance_ip.

An important note is that it is necessary to run terraform apply before you run this command in order to produce accurate results.

- `terraform taint`

This command marks resources which have been altered outside of the scope of terraform. Once the resource has been highlighted, it is deleted and recreated according to the configuration files the next time terraform apply is run. 















