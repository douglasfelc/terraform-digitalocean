# Using Terraform in DigitalOcean

This is a simple example of using Terraform in DigitalOcean.

The file with the Terraform variables `terraform.tfvars` must be created, and declared the following variables:

do_token     = ""
ssh_key_name = ""
region       = ""

Since, `do token` is the DigitalOcean API access token, `ssh_key_name` is the name of the ssh key configured to access the resource and `region` is the region where the resources must be created.

## Basic Terraform Commands

The terraform init command initializes a working directory containing Terraform configuration files.
Also install new providers when needed.
```
terraform init
```

Format the file
```
terraform fmt
```

Shows the execution plan
```
terraform plan
```

Apply the infrastructure declared in the file
```
terraform apply
```

Destroys the infrastructure declared in the file
```
terraform destroy
```