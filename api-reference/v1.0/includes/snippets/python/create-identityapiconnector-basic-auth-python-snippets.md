---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = IdentityApiConnector(
	display_name = "Test API",
	target_url = "https://someapi.com/api",
	authentication_configuration = BasicAuthentication(
		odata_type = "#microsoft.graph.basicAuthentication",
		username = "MyUsername",
		password = "MyPassword",
	),
)

result = await graph_client.identity.api_connectors.post(request_body)


```