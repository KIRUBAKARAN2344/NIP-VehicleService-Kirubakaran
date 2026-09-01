# 🚗 Vehicle Service Management Application

<p align="center">
  <img src="https://img.shields.io/badge/Pega-Platform-0070AD?style=for-the-badge&logo=pega&logoColor=white" />
  <img src="https://img.shields.io/badge/Project-National%20Internship%20Program-6A1B9A?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Workflow-Automation-FF6F00?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Prototype-2E7D32?style=for-the-badge" />
</p>

<p align="center">
  <b>A Pega-based Vehicle Service Workflow Automation Solution</b>
</p>

<p align="center">
  Manage vehicle service requests from customer intake through assessment,
  approval, service execution, and completion.
</p>

---

## 🌟 Project Overview

The **Vehicle Service Management Application** is a workflow automation solution developed using **Pega Platform** as part of the **National Internship Program (NIP)**.

The application manages the lifecycle of a vehicle service request through a structured case-management workflow:

```text
Request Intake
      ↓
Assessment
      ↓
Approval
      ↓
Service Execution
      ↓
Completion
      ↓
Customer Handover
```

---

## 🎯 Problem Statement

Vehicle servicing involves multiple activities including customer request submission, vehicle assessment, service estimation, approval, technician assignment, service execution, and final completion.

When these activities are handled manually or through disconnected processes, organizations can experience delays, inconsistent information, communication gaps, and limited visibility into the service lifecycle.

This project demonstrates how a centralized Pega case-management workflow can organize and automate the vehicle-service process.

---

## 💡 Project Objectives

- 🚗 Manage vehicle service requests
- 🔍 Perform structured vehicle assessment
- 💰 Manage service estimates and costs
- ✅ Support approval workflow
- 👨‍🔧 Support technician assignment
- 🔀 Route requests based on vehicle type
- ⏱️ Support service-level requirements
- 📩 Manage service completion
- 📊 Improve case visibility
- 🤝 Provide a structured service lifecycle

---

## 🏗️ Application Architecture

```text
                    ┌─────────────────────┐
                    │      Customer       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Pega Application  │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
        Request Intake    Assessment        Approval
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                    ┌─────────────────────┐
                    │  Service Execution  │
                    └──────────┬──────────┘
                               │
                    ┌──────────┴──────────┐
                    ▼                     ▼
             Vehicle Routing        Technician Work
                    │                     │
                    └──────────┬──────────┘
                               ▼
                    ┌─────────────────────┐
                    │      Completion     │
                    └──────────┬──────────┘
                               ▼
                    ┌─────────────────────┐
                    │  Customer Handover  │
                    └─────────────────────┘
```

---

## 🔄 Case Lifecycle

### 1️⃣ Request Intake
A service request is created with the required vehicle and service information.

### 2️⃣ Assessment
Vehicle inspection and assessment information is captured.

### 3️⃣ Approval
The service estimate is reviewed and approval is obtained where required.

### 4️⃣ Service Execution
The approved request proceeds to service execution and technician processing.

### 5️⃣ Completion
The completed service request proceeds through final completion and customer handover.

---

## 📋 User Stories

The NIP Vehicle Service application is organized around the required user stories:

| ID | User Story |
|---|---|
| 🟢 US-001 | Submit Vehicle Service Request |
| 🟢 US-002 | Perform Vehicle Inspection |
| 🟢 US-003 | Generate Service Estimate |
| 🟢 US-004 | Approve Service Estimate |
| 🟢 US-005 | Maintain Vehicle Data |
| 🟢 US-006 | Review Service Estimate |
| 🟢 US-007 | Auto Assign Technician |
| 🟢 US-008 | Notify Service Completion |
| 🟢 US-009 | Define Service SLA |
| 🟢 US-010 | Route by Vehicle Type |

> The exact implementation and evidence for each story should be verified against the completed Pega application and NIP submission document.

---

## ⚙️ Key Capabilities

### 🚗 Vehicle Service Requests
Structured creation and management of vehicle service cases.

### 🔍 Vehicle Assessment
Captures inspection and assessment information as part of the case lifecycle.

### 💰 Service Cost Management
Supports service estimate and total-cost handling.

### ✅ Approval Workflow
Moves applicable service requests through an approval stage.

### 👨‍🔧 Technician Assignment
Supports assignment of service work to technicians.

### 🔀 Vehicle-Type Routing
Supports routing based on vehicle characteristics.

### ⏱️ SLA Management
Supports service-level requirements for case processing.

### 📩 Completion Handling
Supports the final service completion and customer handover process.

---

## 👥 Personas

The application documentation includes personas such as:

- 👨‍💼 Financial Officer
- 👤 Individual Owner
- 👨‍🔧 Service Technician
- 👥 Users

---

## 🗂️ Work Queues

Work can be organized using appropriate Pega work queues for vehicle-service processing, including vehicle-type-specific routing where configured.

---

## 🧠 Pega Platform

This project demonstrates Pega case-management and workflow capabilities.

### Platform Components

- Pega App Studio
- Pega Dev Studio
- Case Management
- Case Types
- Workflow Stages
- Personas
- Work Queues
- Business Rules
- Approvals
- Routing
- SLA configuration

---

## 🧪 Testing & Evidence

The application has been tested using vehicle service cases through the configured workflow.

Project evidence should be maintained in:

```text
Screenshots/
```

Recommended evidence organization:

```text
Screenshots/
├── US-001.png
├── US-002.png
├── US-003.png
├── US-004.png
├── US-005.png
├── US-006.png
├── US-007.png
├── US-008.png
├── US-009.png
└── US-010.png
```

Use only screenshots that genuinely represent the implemented Pega application.

---

## 📦 Pega Application Export

The repository can contain the Pega-generated application export under:

```text
Pega-Export/
```

Typical exported artifacts may include:

```text
Application.xml
application.properties
META-INF/
*_rules.jar
*_schema.jar
```

These files should be kept as generated by Pega and should not be manually modified.

---

## 📄 Documentation

Project documentation and NIP evidence should be maintained under:

```text
Documentation/
```

Recommended contents:

- Completed NIP submission document
- User-story evidence
- Application screenshots
- Project description
- Testing evidence
- Pega configuration notes

---

## 🎥 Demo

**Demo video:** Coming soon

The final demo should demonstrate the working application, case creation, major workflow stages, important business rules, and successful case completion.

---

## 🔗 Project Links

### GitHub Repository

**Vehicle Service Management Application**

https://github.com/KIRUBAKARAN2344/NIP-VehicleService-Kirubakaran

### Pega Application

The working application is maintained in the assigned Pega environment.

### Demo Video

Coming soon.

---

## 🛠️ Technology & Tools

| Technology | Purpose |
|---|---|
| **Pega Platform** | Application development |
| **App Studio** | Low-code application development |
| **Dev Studio** | Advanced configuration |
| **Case Management** | Workflow management |
| **Business Rules** | Process automation |
| **Work Queues** | Work assignment |
| **SLA** | Service-level management |

---

## 📈 Future Enhancements

Potential future enhancements include:

- 🤖 AI-assisted service estimation
- 🔧 Predictive maintenance integration
- 📊 Advanced service analytics
- 🔔 Real-time customer notifications
- 🧠 AI-assisted technician recommendation
- 🚘 Predictive service recommendations
- 🔗 Automotive service API integration
- 📡 IoT-based vehicle diagnostics

> These are future enhancement ideas and should not be presented as currently implemented features unless they have actually been built and tested.

---

## 👨‍💻 Project Author

### KIRUBAKARAN M

**B.E. Computer Science and Engineering (AI & ML)**

**V.S.B. Engineering College**

Tamil Nadu, India

---

## 🏆 National Internship Program

This project was developed as part of the **Pega National Internship Program**.

The repository is intended to provide supporting project artifacts, documentation, evidence, and the Pega application export where permitted.

---

## 🔐 Security

Do not commit:

- Passwords
- API keys
- Authentication tokens
- Private credentials
- Confidential environment information
- Sensitive personal information

---

<p align="center">
  <b>🚗 Vehicle Service Management Application</b><br>
  Built with Pega Platform | National Internship Program
</p>
