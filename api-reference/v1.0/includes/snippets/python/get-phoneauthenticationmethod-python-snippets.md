---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.me.authentication.phone_methods.by_phone_authentication_method_id('phoneAuthenticationMethod-id').get()


```