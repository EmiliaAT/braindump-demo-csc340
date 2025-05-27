# Software Requirements Specification
## For BrainDump

Version 0.1  
Prepared by Emilia Trickett and Sebastian Foreman UNCG CSC-340 5/26/2025

Table of Contents
=================
* [Revision History](#revision-history)
* 1 [Introduction](#1-introduction)
  * 1.1 [Document Purpose](#11-document-purpose)
  * 1.2 [Product Scope](#12-product-scope)
  * 1.3 [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
  * 1.4 [References](#14-references)
  * 1.5 [Document Overview](#15-document-overview)
* 2 [Product Overview](#2-product-overview)
  * 2.1 [Product Functions](#21-product-functions)
  * 2.2 [Product Constraints](#22-product-constraints)
  * 2.3 [User Characteristics](#23-user-characteristics)
  * 2.4 [Assumptions and Dependencies](#24-assumptions-and-dependencies)
* 3 [Requirements](#3-requirements)
  * 3.1 [Functional Requirements](#31-functional-requirements)
    * 3.1.1 [User Interfaces](#311-user-interfaces)
    * 3.1.2 [Hardware Interfaces](#312-hardware-interfaces)
    * 3.1.3 [Software Interfaces](#313-software-interfaces)
  * 3.2 [Non-Functional Requirements](#32-non-functional-requirements)
    * 3.2.1 [Performance](#321-performance)
    * 3.2.2 [Security](#322-security)
    * 3.2.3 [Reliability](#323-reliability)
    * 3.2.4 [Availability](#324-availability)
    * 3.2.5 [Compliance](#325-compliance)
    * 3.2.6 [Cost](#326-cost)
    * 3.2.7 [Deadline](#327-deadline)

## Revision History
| Name | Date    | Reason For Changes  | Version   |
| ---- | ------- | ------------------- | --------- |
|  Sebastian F    |    5/26     |  2.3,2.4,3.2 completed |  v0.1  |
|      |         |                     |           |
|      |         |                     |           |

## 1. Introduction

### 1.1 Document Purpose

### 1.2 Product Scope

### 1.3 Definitions, Acronyms and Abbreviations                                                                                                                                                                          |

### 1.4 References

### 1.5 Document Overview

## 2. Product Overview

### 2.1 Product Functions

### 2.2 Product Constraints

### 2.3 User Characteristics
Users will be divided into two different roles: authors or readers.
Authors will publish content and readers will comment upon that content.

### 2.4 Assumptions and Dependencies
The application is dependent upon third party hosting of PostgreSQL providing interactive response times over the open internet.

## 3. Requirements

### 3.1 Functional Requirements 

#### 3.1.1 User interfaces
Web pages using HTML, CSS, and JavaScript.

#### 3.1.2 Hardware interfaces
Devices that have web browser capabilities.

#### 3.1.3 Software interfaces
- Java jdk 21
- PostgreSQL 17
- SpringBoot 3.4.5
- 
### 3.2 Non Functional Requirements 

#### 3.2.1 Performance
- 1: BrainDump will require less than 200 MB of working memory and less than 1 GB of persistent storage.
- 2: Application will support interactive response times of less than 10 seconds round trip.
- 3: New users will be able to create and publish a basic article without prior instruction.

#### 3.2.2 Security
- 4: Username and password authentication will be performed for any action that modifies data.

#### 3.2.3 Reliability
- 5: The application will possess 100% unit test coverage for all functionality.

#### 3.2.4 Availability
- 6: BrainDump will be available 24 hours a day, 7 days a week. Unless maintenence windows are explicitly booked with prior user notification. 

#### 3.2.5 Compliance
- 7: No personal data beyond email address will be maintained by the application.
- 8: No financial data will be retained by the application.
- 9: Users will be warned not to publish personal data within articles.

#### 3.2.6 Cost
- 10: No costs are permitted beyond the unpaid labor provided by the contributors

#### 3.2.7 Deadline
- 11: The final product and associated documentation will be delivered on June 18th.
