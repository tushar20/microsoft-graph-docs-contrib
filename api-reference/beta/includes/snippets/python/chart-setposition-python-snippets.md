---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = SetPositionPostRequestBody(
	start_cell = "startCell-value",
	end_cell = "endCell-value",
)

await graph_client.drives.by_drive_id('drive-id').items.by_drive_item_id('driveItem-id').workbook.worksheets.by_workbook_worksheet_id('workbookWorksheet-id').charts.by_workbook_chart_id('workbookChart-id').set_position.post(request_body)


```