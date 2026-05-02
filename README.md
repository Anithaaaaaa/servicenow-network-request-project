# 🚀 Automated Network Request Management in ServiceNow

## 📌 Project Overview

This project demonstrates a simplified Automated Network Request Management system built on the ServiceNow platform.
It allows users to submit network-related requests through the Service Catalog, which are automatically processed and assigned to the support team without manual intervention.

---

## 🎯 Objectives

* To automate the request handling process
* To reduce manual effort in task creation
* To demonstrate ServiceNow core functionalities
* To simulate real-world IT service management (ITSM) workflow

---

## 🛠️ Technologies Used

* ServiceNow Platform
* Service Catalog
* Catalog Client Scripts
* Business Rules
* Tables: sc_req_item, sc_task

---

## ⚙️ Features Implemented

* ✅ Custom Service Catalog Item (Network Request)
* ✅ Dynamic form behavior using Client Script
* ✅ Automatic task creation using Business Rule
* ✅ Task assignment to Network Team
* ✅ End-to-end request lifecycle tracking
* ✅ No Flow Designer used (simplified approach)

---

## 🔄 Workflow

User submits request
⬇
Request (REQ) is created
⬇
Requested Item (RITM) is generated
⬇
Business Rule triggers
⬇
Task (TASK) is automatically created
⬇
Task assigned to Network Team
⬇
Task processed and closed

---

## 📋 Implementation Steps

### 1. Service Catalog Setup

* Created "Network Request" catalog item
* Added variables:

  * Request Type
  * Access Level
  * Device
  * Business Justification

### 2. User Groups

* Created:

  * Network Team
  * Requesters
* Added users to groups

### 3. Client Script

* Implemented onChange script
* Dynamically shows/hides device field

### 4. Business Rule

* Table: Requested Item (sc_req_item)
* Trigger: After Insert
* Function: Automatically creates a catalog task

### 5. Task Handling

* Task assigned to Network Team
* Updated task status:

  * Work in Progress
  * Closed Complete

---


## 🎥 Demo Video
https://drive.google.com/file/d/1gR8W96RE02_BHCIa6PdElsR2WBoTAVZk/view?usp=drivesdk

---

## 💡 Key Learnings

* Understanding ServiceNow data model (REQ, RITM, TASK)
* Implementing automation using Business Rules
* Creating dynamic UI using Client Scripts
* Managing Service Catalog items
* Handling request lifecycle

---

## 📊 Future Enhancements

* Add approval workflow
* Implement notifications
* Add SLA tracking
* Use Flow Designer for advanced automation

---

## 🏁 Conclusion

This project successfully demonstrates how network requests can be automated in ServiceNow using simple and efficient techniques without relying on complex workflows. It provides a strong foundation for understanding ITSM processes.

---

## 👨‍💻 Author

Anitha
3BR22EC009

---

