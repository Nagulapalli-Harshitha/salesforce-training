# Chapter 12 — Placement Management System

## Overview

Chapter 12 demonstrates a Salesforce Placement Management System project using Salesforce DX, Lightning Web Components (LWC), custom objects, Git, and Salesforce CLI.

The project includes a custom `Application__c` object for managing placement applications and a `placementHome` Lightning Web Component.

## Project Structure

```text
PlacementPortal/
├── force-app/
│   └── main/
│       └── default/
│           ├── lwc/
│           │   └── placementHome/
│           └── objects/
│               └── Application__c/
├── config/
├── scripts/
├── package.json
├── package-lock.json
├── sfdx-project.json
└── README.md
