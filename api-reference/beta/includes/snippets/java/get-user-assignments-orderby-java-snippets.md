---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().me().assignments()
	.buildRequest()
	.orderBy("status")
	.get();

```