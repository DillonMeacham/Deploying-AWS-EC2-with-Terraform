<h1>Deploying an AWS EC2 Instance with Terraform</h1>

<h2>Description</h2>
Terraform is an open-source infrastructure as code (IaC) tool that enables you to safely and predictably create, change, and improve infrastructure. In this project, we will be creating a VM in AWS by following the Terraform workflow, Write > Plan > Apply. After we have successfully deployed the VM, we will then clean up our infrastructure and destroy it :) Let's get started.

<br />

<img src="https://imgur.com/0SNiQ6J.png" height="30%" width="30%" />


<h2>Environments Used </h2>

- <b>Terraform</b>
- <b>Local Command Prompt</b>
- <b>AWS Management Console</b>

<h2>Project walk-through:</h2>

<h2>First we need to SSH into our machine.
<br />
<br />
<img src="https://imgur.com/L24JqzA.png" height="80%" width="80%">
<br />
<br />

We now need to create a directory to house our Terraform code, we'll call the directory 
"terraform_code".
<br />
<br />
<img src="https://imgur.com/LiLzAIG.png" height="80%" width="80%">
<br />
<br />


Then we create a new file for the code called main.tf by using the command 'vim main.tf'. And then add the code for creating an EC2 instance in AWS to the main.tf file.
<br />
<br />
<img src="https://imgur.com/6cYa7Fj.png" height="80%" width="80%">
<br />
<br />
Now we need to initialize the Terraform configuration with the 'terraform init' command. Which initializes our working directory containing the configuration files (main.tf) and installs plugins for required providers.
<br />
<br />
<img src="https://imgur.com/wsGUnaR.png" height="80%" width="80%">
<br />
<br />

After initializing, we need to run the 'terraform plan' command to create an execution plan, which lets you preview the changes that Terraform plans to make to your infrastructure.
<br />
<br />
<img src="https://imgur.com/D9rfgeM.png" height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/o0FkyL7.png" height="80%" width="80%">
<br />
<br />
Now that we have a plan set, we can now execute that plan with 'terraform apply' which will create our instance in AWS.
<br />
<br />
<img src="https://imgur.com/IvPX2Bn.png" height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/AC4dV3U.png" height="80%" width="80%">
<br />
<br />
Let's check the AWS management console to see if our EC2 instances has been created. Looks like it did!
<br />
<br />
<img src="https://imgur.com/bzEEVYN.png" height="80%" width="80%">
<br />
<br />
Finally, we can destroy our infrastructure using the 'terraform destroy' command.
<br />
<br />
<img src="https://imgur.com/FnHiqxD.png" height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/KCeJVv7.png" height="80%" width="80%">
<br />
<br />
<h2>I hope you enjoyed following along if you did!<h2>
