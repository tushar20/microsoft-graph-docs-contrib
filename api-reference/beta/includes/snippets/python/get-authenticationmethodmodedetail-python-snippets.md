---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.identity.conditional_access.authentication_strength.authentication_method_modes.by_authentication_method_mode_detail_id('authenticationMethodModeDetail-id').get()


```