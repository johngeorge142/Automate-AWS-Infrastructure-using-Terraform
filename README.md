**Automate AWS Infrastructure using Terraform**

The purpose of this project is to create an entire AWS Infrastructure using Terraform. The entire project will be built using Infrastucture as Code without manually provisioning resources on the AWS platform. By utilizing terraform, we wil be able to create VPC's for production and test environments and serving web-servers for production and testing in those subnets using tags. We will also create different routes for those subnets using routing tables and internet gateways to route traffic to and from subnets while using a secure tunnel to allow ingress and egress traffic. We will also create network interfaces and elastic IP addresses for those interfaces to be able to point our web servers to specific IP addresses. By creating these resources through code we will be able to automate our entire infrastucture and create,modify and delete resources using Terraform.

**How to Install Terraform**

Homebrew is a free and open-source package management system for Mac OS X. Install the official Terraform formula from the terminal.

First, install the HashiCorp tap, a repository of all our Homebrew packages.

$ brew tap hashicorp/tap
Copy
Now, install Terraform with hashicorp/tap/terraform.

$ brew install hashicorp/tap/terraform
Copy
NOTE: This installs a signed binary and is automatically updated with every new official release.
To update to the latest version of Terraform, first update Homebrew.

$ brew update
Copy
Then, run the upgrade command to download and use the latest Terraform version.

$ brew upgrade hashicorp/tap/terraform
==> Upgrading 1 outdated package:
hashicorp/tap/terraform 0.15.3 -> 1.0.0
==> Upgrading hashicorp/tap/terraform 0.15.3 -> 1.0.0
Copy
»Verify the installation

Verify that the installation worked by opening a new terminal session and listing Terraform's available subcommands.

$ terraform -help
Usage: terraform [-version] [-help] <command> [args]

The available commands for execution are listed below.
The most common, useful commands are shown first, followed by
less common or more advanced commands. If you're just getting
started with Terraform, stick with the common commands. For the
other commands, please read the help and docs before usage.
##...
Copy
Add any subcommand to terraform -help to learn more about what it does and available options.

$ terraform -help plan

**How to use the project**

1. First run terraform init to initialize terraform
2. Use terraform plan
3. Use terraform apply to create the resources
