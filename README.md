# Terraform_VM-Create

1) Defined Terraform required_providers version to use.
2) Created service principal on Azure Cloud and assigned contributor role. Created secret for the SP.
3) Provider definitions have been updated with subscription_id, client_id, tenant_id and client secret.
4)  Resource group define and provided the location to use while creating the VM.
5)  Network Security group resource create and rule to allow inbound treaffic to 22 port has been defined.
6)  Public Ip resource defined. This would be the Ip of Azure VM to connect.
7)  Virtual Network and subnets defined.
8)  Network Interface resource with Ip configuration and publick key association defined.
9)  Azure and Terraform handle NSG binding to NICs using a separate resource called azurerm_network_interface_security_group_association. Define this resourced.
10)  azurerm_linux_virtual_machine resource defined to launch the VM.
