# 📋 BRD & FRD: Business & Functional Requirements Documents

Understanding requirements is one of the most important parts of the **Software Development Life Cycle (SDLC)**. Two documents commonly used to capture and communicate these requirements are the **BRD** and **FRD**.

> 💡 **In simple terms:**
> **BRD defines *****what the business needs and why*****.**
> **FRD defines *****what the system should do to fulfill those needs*****.**

---

## 📌 What is BRD?

**BRD** stands for **Business Requirements Document**.

A BRD describes the **high-level business requirements** of a software project. It focuses primarily on the **business perspective**, explaining what the organization wants to achieve and why the project is necessary.

### 🎯 Purpose of a BRD

The BRD typically defines:

* 🎯 **Business goals and objectives**
* 📌 **Project scope**
* 📦 **Expected deliverables**
* 👥 **Stakeholder requirements**
* ⚠️ **Business constraints**
* 💭 **Assumptions**
* 📈 **Expected business outcomes**

The document is generally prepared by **Business Analysts or Project Managers** in collaboration with stakeholders.

### 🗺️ BRD as a Project Roadmap

The BRD acts as a **roadmap for the project**, helping everyone understand:

> **What does the business want to achieve?**

It provides the foundation from which more detailed system requirements can be derived.

### 📝 Typical BRD Structure

```
Business Requirement Document
│
├── 1. Introduction
│   ├── Purpose
│   ├── Background
│   └── Document Objectives
│
├── 2. Business Objectives
│
├── 3. Project Scope
│   ├── In Scope
│   └── Out of Scope
│
├── 4. Stakeholders
│
├── 5. Business Requirements
│
├── 6. Business Rules
│
├── 7. Assumptions & Constraints
│
├── 8. Risks
│
└── 9. Approval & Sign-off
```
---

## ⚙️ What is FRD?

**FRD** stands for **Functional Requirements Document**.

An FRD describes the **detailed functional requirements** of a software system. It translates business requirements into specific system behaviors and functionalities that developers, testers, and other technical team members can understand.

### 🔧 Purpose of an FRD

The FRD typically defines:

* ⚙️ **System features**
* 🧩 **Functional requirements**
* 🔄 **System workflows**
* 📥 **Inputs and outputs**
* 🚦 **Business rules**
* 🔐 **Security requirements**
* ⚡ **Performance requirements**
* 🛠️ **Technical specifications**
* ✅ **Expected system behavior**

The FRD may be created by **Software Architects, Developers, QA Engineers, or Business Analysts**, depending on the organization's process, in collaboration with stakeholders and based on the BRD.

### 🏗️ FRD as a System Blueprint

The FRD acts as a **blueprint for the development team**, helping them understand:

> **What needs to be built, and how should it function?**

It provides enough detail for developers to implement the required functionality and for QA engineers to design appropriate test scenarios and test cases.

### 📝 Typical FRD Structure

```
Functional Requirement Document
│
├── 1. Introduction
│
├── 2. Reference to BRD
│
├── 3. System Overview
│
├── 4. Functional Requirements
│   ├── User Registration
│   ├── Login
│   ├── Password Reset
│   └── User Management
│
├── 5. Business Rules
│
├── 6. Input & Output Requirements
│
├── 7. Validation Rules
│
├── 8. Error Handling
│
├── 9. System Workflows
│
└── 10. Approval & Sign-off
```
---

## 🔍 BRD vs FRD

| Aspect               | BRD                                                 | FRD                                                         |
| -------------------- | --------------------------------------------------- | ----------------------------------------------------------- |
| **Full Form**        | Business Requirements Document                      | Functional Requirements Document                            |
| **Focus**            | Business needs                                      | System functionality                                        |
| **Perspective**      | Business                                            | Technical / Functional                                      |
| **Main Question**    | What does the business need and why?                | How should the system function?                             |
| **Level of Detail**  | High-level                                          | Detailed                                                    |
| **Primary Audience** | Stakeholders, Business Analysts, Project Managers   | Developers, QA Engineers, Architects                        |
| **Defines**          | Goals, objectives, scope, and business requirements | Features, workflows, behaviors, and functional requirements |
| **Based On**         | Business needs and stakeholder expectations         | BRD and stakeholder requirements                            |
| **Used For**         | Project direction and business alignment            | Development and testing                                     |
| **Output**           | Business requirements                               | Functional system specifications                            |

---

## 🔗 How BRD and FRD Are Connected

The relationship between the two documents can be represented as:

```text
┌───────────────────────────────┐
│       Business Needs          │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│             BRD               │
│  Business Requirements        │
│  What & Why                   │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│             FRD               │
│  Functional Requirements      │
│  What the system must do      │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│       Design & Development    │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│          QA & Testing         │
└───────────────────────────────┘
```

### 💡 A Simple Example

Imagine a company wants to develop an **online banking application**.

#### BRD might state:

> **Business Requirement:**
> Customers should be able to transfer money to other bank accounts online without visiting a physical branch.

This describes **what the business wants and why**.

#### FRD might define:

* Users must be able to enter a recipient account number.
* Users must be able to enter the transfer amount.
* The system must validate the recipient account.
* The system must verify the user's available balance.
* The system must require authentication before completing the transfer.
* The system must display a transaction confirmation.
* The system must generate a unique transaction ID.

This describes **how the software should behave to fulfill the business requirement**.

---

## 🎯 BRD → FRD → Development → Testing

A simplified requirements flow looks like this:

```text
Business Requirement
        │
        ▼
       BRD
        │
        ▼
Functional Requirements
        │
        ▼
       FRD
        │
        ▼
System Design & Development
        │
        ▼
       QA Testing
        │
        ▼
       Final Product
```

This traceability helps ensure that the final software product remains aligned with the original **business objectives**.

---

## 🧪 Why BRD and FRD Matter to QA Engineers

Both documents can be valuable references for **Software Quality Assurance (SQA)**.

### BRD helps QA understand:

* Why the software is being developed
* What business objectives must be achieved
* What is within and outside the project scope
* Who the stakeholders are
* What the expected business outcomes are

### FRD helps QA understand:

* What features need to be tested
* How each feature should behave
* Expected inputs and outputs
* Business rules and validations
* Functional dependencies
* Error-handling requirements
* Security and performance expectations

QA engineers can use these requirements to derive:

```text
BRD / FRD
    │
    ├── Test Scenarios
    │
    ├── Test Cases
    │
    ├── Test Data
    │
    ├── Acceptance Criteria
    │
    └── Traceability
```

---

## 📝 BRD vs FRD: The Key Difference

The easiest way to remember the difference is:

> 🏢 **BRD = Business Perspective**
> **What does the business need, and why?**

> 💻 **FRD = Functional Perspective**
> **What should the system do to satisfy that need?**

### In one sentence:

**BRD defines the business requirements at a high level, while FRD translates those requirements into detailed functional specifications that guide development and testing.**

---

## 🚀 Final Takeaway

BRD and FRD serve different but interconnected purposes throughout the software development process.

**BRD** establishes the **business direction** by describing the goals, objectives, scope, and high-level requirements.

**FRD** takes those business requirements and translates them into **specific functional requirements**, giving the development and QA teams a clearer understanding of what the system needs to do.

Together, they help bridge the gap between:

**Business Expectations → Technical Implementation → Quality Assurance**

Understanding this relationship is especially important for **Business Analysts, Developers, QA Engineers, Project Managers, and other stakeholders** involved in the SDLC.
