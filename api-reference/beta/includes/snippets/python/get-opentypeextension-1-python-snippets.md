---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.me.messages.by_message_id('message-id').extensions.by_extension_id('extension-id').get()


```