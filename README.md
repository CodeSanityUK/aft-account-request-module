<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.15.1 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 3.15 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 3.15 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_dynamodb_table_item.account-request](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table_item) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_account-request-table"></a> [account-request-table](#input\_account-request-table) | name of account-request-table | `string` | `"aft-request"` | no |
| <a name="input_account-request-table-hash"></a> [account-request-table-hash](#input\_account-request-table-hash) | name of account-request-table hash key | `string` | `"id"` | no |
| <a name="input_account_customizations_name"></a> [account\_customizations\_name](#input\_account\_customizations\_name) | The name of the account customizations to apply | `string` | `""` | no |
| <a name="input_account_tags"></a> [account\_tags](#input\_account\_tags) | map of account-level tags | `map(any)` | `{}` | no |
| <a name="input_change_management_parameters"></a> [change\_management\_parameters](#input\_change\_management\_parameters) | n/a | <pre>object({<br>    change_requested_by = string<br>    change_reason       = string<br>  })</pre> | n/a | yes |
| <a name="input_control_tower_parameters"></a> [control\_tower\_parameters](#input\_control\_tower\_parameters) | n/a | <pre>object({<br>    AccountEmail              = string<br>    AccountName               = string<br>    ManagedOrganizationalUnit = string<br>    SSOUserEmail              = string<br>    SSOUserFirstName          = string<br>    SSOUserLastName           = string<br>  })</pre> | n/a | yes |
| <a name="input_custom_fields"></a> [custom\_fields](#input\_custom\_fields) | map of custom fields defined by the customer | `map(any)` | `{}` | no |

## Outputs

No outputs.
<!-- END_TF_DOCS -->