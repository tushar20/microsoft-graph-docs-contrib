---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.device_management.device_configurations.by_device_configuration_id('deviceConfiguration-id').user_statuses.by_device_configuration_user_status_id('deviceConfigurationUserStatus-id').get()


```