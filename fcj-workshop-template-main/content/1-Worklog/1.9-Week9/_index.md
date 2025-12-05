---
title: "Week 9 Worklog"
date: "2025-11-03"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Week 9 Objectives:

* Implement Hybrid Authentication (Fingerprint + Cloud).
* Build API for data retrieval (Dashboard & Search).
* Complete business logic layer.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                            | Start Date | Completion Date |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| 1   | - Create DynamoDB DeviceOfficerMap_Pool table <br> - Write Lambda AuthorizeFunction for fingerprint verification                                                                                | 03/11/2025 | 03/11/2025      |
| 2   | - Configure IoT Rule for authorization flow <br> - Update ESP32 firmware: Scan fingerprint → Send SlotID → Receive unlock command                                                              | 04/11/2025 | 04/11/2025      |
| 4   | - Create 2 GSI on ViolationsDB (Dashboard & Search indexes) <br> - Write Lambda GetDashboardFunction and SearchByCCCDFunction                                                                   | 06/11/2025 | 07/11/2025      |

| Day | Event/Task | Date | Format | Key Activities & Outcomes |
| --- | ---------- | ---- | ------ | ------------------------- |
| 6   | **Team Meeting #2**<br/>*API Integration Testing* | 08/11/2025 | Offline | **Focus:**<br/>• Test fingerprint authentication end-to-end<br/>• Debug API Lambda functions<br/>• Validate GSI query performance<br/><br/>**Results:**<br/>✓ Fingerprint auth working correctly<br/>✓ APIs returning proper JSON data |

| Day | Task                                                                                                                                                                                            | Start Date | Completion Date |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| 7   | - Setup API Gateway: Create /dashboard and /search/{cccd} endpoints <br> - Enable CORS configuration <br> - Integration test: Browser → API → JSON response <br> - Write worklog and review week progress | 09/11/2025 | 09/11/2025      |


### Week 9 Achievements:

* **Authentication**: Fingerprint scan → Device unlocks successfully.
* **API Layer**: Dashboard and Search endpoints operational.
* **Database**: GSI indexes optimized for query patterns.
* **Deliverable**: Browser API call returns violation data in JSON format.
