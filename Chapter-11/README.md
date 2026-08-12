# Chapter 11 – Candidate Recruitment API Integration

## Overview

Chapter 11 implements an external candidate recruitment API integration in Salesforce.

The integration uses Apex Queueable to perform an asynchronous HTTP callout when an Application record is selected. A mock recruitment API is used for testing the integration without depending on a real external backend.

## Features

- External Recruitment API integration
- Salesforce Named Credential
- External Credential
- Asynchronous processing using Queueable Apex
- HTTP POST callout
- Application Trigger
- Success and error handling
- Retry handling for server errors
- Comprehensive Apex test coverage
- Mock API using Beeceptor
- Lightning Web Component for placement functionality

## Integration Flow

```text
Application Record
        |
        | Status changed to Selected
        v
ApplicationTrigger
        |
        v
CandidateSyncQueueable
        |
        v
Named Credential
Recruitment_API
        |
        v
POST /candidates
        |
        v
Beeceptor Mock API
        |
        v
HTTP Response
        |
        +----------------------+
        |                      |
      201                    Error
        |                      |
        v                      v
Integration Status        Error Handling
= Sent                   / Retry Required
        |
        v
External Candidate ID