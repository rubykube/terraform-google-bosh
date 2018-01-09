# GCP BOSH module

Base infrastructure for a BOSH deployment on GCP

## Usage

To use the module, just append the following lines to your Terraform files and fill in proper values

```ruby
module "bosh" {
  source                = "github.com/rubykube/terraform-google-bosh"
  project               = "example-project"
  region                = "us-west1"
  zone                  = "us-west1-c"
  vpc_name              = "example-cloud"
  platform_subnet_name  = "platform-example"
  subnet_cidr           = "10.0.20.0/24"
  public_key            = "~/.ssh/key.pub"
}
```
