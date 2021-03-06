Terraform module which creates ALB instance on Alibaba Cloud.

terraform-alicloud-alb
=====================================================================

English | [简体中文](https://github.com/terraform-alicloud-modules/terraform-alicloud-alb/blob/master/README-CN.md)

Terraform module which creates ALB and enables logs configuration on Alibaba Cloud.

These types of resources are supported:

* [Alb_Load_Balancer](https://registry.terraform.io/providers/aliyun/alicloud/latest/docs/resources/alb_load_balancer)

## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | > = 0.13.0 |
| <a name="requirement_alicloud"></a> [alicloud](#requirement\_alicloud) | > = 1.131.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_alicloud"></a> [alicloud](#provider\_alicloud) | > = 1.131.0 |

## Usage

```hcl
module "example" {
  source                     = "terraform-alicloud-modules/alb/alicloud"
  vpc_name                   = "tf_vpc_name"
  vpc_cidr_block             = "11.0.0.0/16"
  alb_address_type           = "Internet"
  alb_address_allocated_mode = "Fixed"
  alb_load_balancer_name     = "tf_alb_name"
  alb_load_balancer_edition  = "Basic"
}
```

Submit Issues
-------------
If you have any problems when using this module, please opening
a [provider issue](https://github.com/aliyun/terraform-provider-alicloud/issues/new) and let us know.

**Note:** There does not recommend to open an issue on this repo.

Authors
-------
Created and maintained by Alibaba Cloud Terraform Team(terraform@alibabacloud.com)

License
----
Apache 2 Licensed. See LICENSE for full details.

Reference
---------

* [Terraform-Provider-Alicloud Github](https://github.com/aliyun/terraform-provider-alicloud)
* [Terraform-Provider-Alicloud Release](https://releases.hashicorp.com/terraform-provider-alicloud/)
* [Terraform-Provider-Alicloud Docs](https://registry.terraform.io/providers/aliyun/alicloud/latest/docs)