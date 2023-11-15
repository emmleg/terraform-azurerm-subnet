<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_azurerm"></a> [azurerm](#provider\_azurerm) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [azurerm_subnet.subnet](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/subnet) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_address_prefixes"></a> [address\_prefixes](#input\_address\_prefixes) | (Required) The address prefixes to use for the subnet. | `list(string)` | n/a | yes |
| <a name="input_delegation"></a> [delegation](#input\_delegation) | (Optional) Delegation configuration for the subnet. | `map(list(any))` | `{}` | no |
| <a name="input_name"></a> [name](#input\_name) | (Required) The name of the subnet. Changing this forces a new resource to be created. | `string` | n/a | yes |
| <a name="input_private_endpoint_network_policies_enabled"></a> [private\_endpoint\_network\_policies\_enabled](#input\_private\_endpoint\_network\_policies\_enabled) | (Optional) Enable or Disable network policies for the private endpoint on the subnet. Setting this to true will Enable the policy and setting this to false will Disable the policy. Defaults to true. | `bool` | `true` | no |
| <a name="input_private_link_service_network_policies_enabled"></a> [private\_link\_service\_network\_policies\_enabled](#input\_private\_link\_service\_network\_policies\_enabled) | (Optional) Enable or Disable network policies for the private link service on the subnet. Setting this to true will Enable the policy and setting this to false will Disable the policy. Defaults to true. | `bool` | `true` | no |
| <a name="input_resource_group_name"></a> [resource\_group\_name](#input\_resource\_group\_name) | (Required) The name of the resource group in which to create the subnet. Changing this forces a new resource to be created. | `string` | n/a | yes |
| <a name="input_service_endpoint_policy_ids"></a> [service\_endpoint\_policy\_ids](#input\_service\_endpoint\_policy\_ids) | (Optional) The list of IDs of Service Endpoint Policies to associate with the subnet. | `list(string)` | `null` | no |
| <a name="input_service_endpoints"></a> [service\_endpoints](#input\_service\_endpoints) | (Optional) The list of Service endpoints to associate with the subnet. Possible values include: Microsoft.AzureActiveDirectory, Microsoft.AzureCosmosDB, Microsoft.ContainerRegistry, Microsoft.EventHub, Microsoft.KeyVault, Microsoft.ServiceBus, Microsoft.Sql, Microsoft.Storage, Microsoft.Storage.Global and Microsoft.Web. | `list(string)` | `[]` | no |
| <a name="input_virtual_network_name"></a> [virtual\_network\_name](#input\_virtual\_network\_name) | (Required) The name of the virtual network to which to attach the subnet. Changing this forces a new resource to be created. | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id"></a> [id](#output\_id) | n/a |
| <a name="output_name"></a> [name](#output\_name) | n/a |
<!-- END_TF_DOCS -->