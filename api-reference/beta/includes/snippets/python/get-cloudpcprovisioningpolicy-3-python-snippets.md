---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = CloudPcProvisioningPolicyItemRequestBuilder.CloudPcProvisioningPolicyItemRequestBuilderGetQueryParameters(
		select = ["id","description","displayName","domainJoinConfiguration","imageDisplayName","imageId","imageType","onPremisesConnectionId","windowsSetting","managedBy","cloudPcGroupDisplayName","gracePeriodInHours","localAdminEnabled","alternateResourceUrl"],
)

request_configuration = CloudPcProvisioningPolicyItemRequestBuilder.CloudPcProvisioningPolicyItemRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.device_management.virtual_endpoint.provisioning_policies.by_cloud_pc_provisioning_policy_id('cloudPcProvisioningPolicy-id').get(request_configuration = request_configuration)


```