# Terraform : EC2

This repo demonstrates the deployment of an EC2 instance via Terraform. Make sure you have both [Terraform](https://www.terraform.io/) and the [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed.


## Setup and Cleanup
Initialize.
```bash
terraform init
```

Plan infrastructure.
```bash
terraform plan
```

Set up the infrastructure.
```bash
terraform apply
```

Tear down the infrastructure.
```bash
terraform destroy
```

## SSH into EC2
Set the permissions on your key.
```bash
chmod 400 retool-key.pem
```

Connect to the instance using the public DNS
```bash
ssh -i "retool-key.pem" ubuntu@ec2-XX-XX-XXX.us-west-2.compute.amazonaws.com
```
