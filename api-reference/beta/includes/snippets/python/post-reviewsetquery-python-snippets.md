---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = ReviewSetQuery(
	display_name = "My Query 1",
	query = "(subject:\"Quarterly Financials\")",
)

result = await graph_client.compliance.ediscovery.cases.by_case_id('case-id').review_sets.by_review_set_id('reviewSet-id').queries.post(request_body)


```