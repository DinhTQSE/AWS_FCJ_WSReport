---
title: "Week 8 Worklog"
date: "2025-10-27"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Week 8 Objectives:

* Build Core Pipeline: Sensor data flows to Database.
* Complete hardware assembly and test all sensors.
* Establish AWS IoT Core connection.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                            | Start Date | Completion Date |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| 1   | - Assemble circuit on Breadboard: ESP32 + MQ-3 + MAX30102 + Keypad + LCD + AS608 <br> - Unit test each sensor individually                                                                     | 27/10/2025 | 28/10/2025      |
| 3   | - Write ESP32 firmware: Read MQ-3 (alcohol) and MAX30102 (heart rate) data <br> - Implement Keypad input and LCD display                                                                       | 29/10/2025 | 30/10/2025      |
| 5   | - Package sensor data as JSON <br> - Implement MQTT publish to AWS IoT Core                                                                                                                     | 31/10/2025 | 31/10/2025      |

| Day | Event/Task | Date | Format | Key Activities & Outcomes |
| --- | ---------- | ---- | ------ | ------------------------- |
| 6   | **Team Meeting #1**<br/>*Hardware & Firmware Sprint* | 01/11/2025 | Offline | **Focus:**<br/>• Debug sensor integration issues<br/>• Test MQTT connection to AWS IoT Core<br/>• Review firmware code quality<br/><br/>**Results:**<br/>✓ All sensors working stable<br/>✓ MQTT successfully publishing data |

| Day | Task                                                                                                                                                                                            | Start Date | Completion Date |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| 7   | - Setup AWS IoT Core: Create Thing, Policy, Certificate <br> - Configure IoT Rule for data routing <br> - Write ProcessViolationFunction Lambda <br> - Create DynamoDB ViolationsDB table <br> - Test end-to-end: Sensor → DynamoDB <br> - Write worklog and review week progress | 02/11/2025 | 02/11/2025      |


### Week 8 Achievements:

* **Hardware**: All sensors operational on breadboard.
* **Firmware**: ESP32 reading sensors and publishing MQTT successfully.
* **AWS**: IoT Core configured, Lambda processing data, DynamoDB storing violations.
* **Deliverable**: Blow into MQ-3 sensor → New record appears in DynamoDB.
