---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = DeleteTiIndicatorsPostRequestBody(
	value = [
		"id-value1",
		"id-value2",
	],
)

result = await graph_client.security.ti_indicators.delete_ti_indicators.post(request_body)


```