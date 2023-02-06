# gcp-terraform-cloud-test-vm
# How-to set up Google Cloud (GCP) credentials in Terraform Cloud

1. As Terraform Variable
```
provider "google" {
  project     = "<YOUR PROJECT>"
  region  = "<YOUR REGION>"
  zone    = "<YOUR ZONE>"
  credentials = var.gcp-creds
}


variable "gcp-creds" {
default= ""
}
```
  
2. Add key in tf cloud as env variable 
   to get key out put without any tabs/spaces
  ```
 cat kk-tf-account.json | jq -c
 ```



Ref: 
# https://support.hashicorp.com/hc/en-us/articles/4406586874387-How-to-set-up-Google-Cloud-GCP-credentials-in-Terraform-Cloud
