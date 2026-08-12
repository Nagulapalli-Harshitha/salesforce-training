# 📚 College Library Management System – Salesforce Mini Project

## Project Overview

The College Library Management System is a Salesforce application developed to automate library operations using declarative Salesforce features such as Custom Objects, Record-Triggered Flows, Validation Rules, and Email Notifications.

This project demonstrates CRM customization and business process automation without extensive coding.

---

## Objectives

- Manage library books and members.
- Track book issue records.
- Maintain fine records.
- Automate issue management.
- Ensure data quality using Validation Rules.
- Notify library administrators automatically.

---

## Custom Objects

1. Book
2. Member
3. Issue Record
4. Fine

---

## Relationships

- Issue Record → Book (Master-Detail)
- Issue Record → Member (Lookup)
- Fine → Issue Record (Master-Detail)

---

## Features Implemented

### 1. Record-Triggered Flow

Created a Record-Triggered Flow that automatically:

- Sets the Issue Date
- Updates the Issue Record
- Sends an email notification
- Creates a Fine record automatically when the Issue Status becomes **Returned**

---

### 2. Validation Rules

Implemented Validation Rules to ensure data quality.

Examples:

- Return Date cannot be earlier than Issue Date.
- Book must be selected before saving.
- Fine Amount cannot be negative.

---

### 3. Automatic Email Notification

Whenever an Issue Record is processed, the system automatically sends an email notification to the Library Administrator.

---

### 4. Automatic Fine Record Creation

When an Issue Record status changes to **Returned**, Salesforce automatically creates a related Fine record.

---

## Automation Used

- Record-Triggered Flow
- Assignment Element
- Update Records Element
- Create Records Element
- Send Email Action
- Validation Rules

---

## Salesforce Concepts Covered

- Custom Objects
- Custom Fields
- Master-Detail Relationship
- Lookup Relationship
- Record-Triggered Flow
- Validation Rules
- Email Alerts
- Create Records
- Update Records
- Flow Debugging

---

## Project Outcome

Successfully automated the library issue management process by:

- Reducing manual work
- Improving data accuracy
- Enforcing business rules
- Automating notifications
- Automatically creating related Fine records

---

## Developed By

**Name:** Nadiminti Manjusha

**Roll Number:** 23PA1A05G6

**Platform:** Salesforce Developer Edition
