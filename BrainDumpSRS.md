# Software Requirements Specification

## BrainDump

**Version:** 0.0.2

**Prepared by:** Emilia Trickett, Sebastian Foreman

**Organisation:** UNCG CSC-340

**Date:** 5/25/2025

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

| Name         | Date    | Reason For Changes      | Version   |
| ------------ | ------- | ----------------------- | --------- |
| Sebastian F. | 5/26/25 | 2.3, 2.4, 3.2 completed | v0.0.1    |
| Emilia T.    | 5/26/25 | Write 1. Introduction   | v0.0.2    |

## 1. Introduction

### 1.1 Document Purpose

The purpose for the Software Requirements Specification is to describe the guest, user, and author client
requirements for the BrainDump web application.

Guest-oriented requirements describe the system from the guest user's perspective. Guest users are those who visit
the BrainDump site without signing in and authenticating. All other user roles share the same capabilities as guests.

User-oriented requirements describe the system from the authenticated user's perspective. All users have access to
everything that guests can do, as well as being able to contribute to the system. Furthermore, while all users have
the ability to be authors, the user role is being defined as it is to support the larger project specification.

Author-oriented requirements describe the system from the authenticated author's perspective. While all users have
access to author capabilities, the author role is defined to demonstrates what requirements must be set in place
to support authorship features for the application.

### 1.2 Product Scope

The BrainDump platform is designed to make writing, storing, and sharing information in the form of educational
articles easy. All articles are composed of simple Markdown, and can be downloaded for offline use at any time.

The platform intentionally has features designed to make finding others' articles easier; using a tagging system,
a collections/albums system, and multiple filtering and sorting options. All authenticated users are able to view articles, create articles publically or privately, and curate articles to their liking.

BrainDump is, above all else, lightweight and accessible for users of all kinds.

### 1.3 Definitions, Acronyms and Abbreviations

| Reference  | Definition                                                                           |
| ---------- | ------------------------------------------------------------------------------------ |
| Java       | The programming language used for the backend server instance.                       |
| TypeScript | The programming language used for the frontend client instance.                      |
| React      | The frontend framework used for the frontend client instance.                        |
| PostgreSQL | The relational database management system used for the backend.                      |
| API        | Application Programming Interface. Used to communicate between backend and frontend. |
| HTML       | HyperText Markup Language. Used to structure the frontend, embedded in TypeScript.   |
| CSS        | Cascading Style Sheets. Used to format the frontend interface.                       |
| VS Code    | One of the text editors used to program the BrainDump platform.                      |
| Neovim     | Another one of the text editors used to program the BrainDump platform.              |
| Git        | The version management control system used to manage the BrainDump platform.         |
| GitHub     | The Git-based developer platform used to host and manage the BrainDump platform.     |

### 1.4 References

N/A.

### 1.5 Document Overview

Section 1 is a general introduction to the document, intended for any readers. Section 2 is focused on the product
and its features. This section is for customers and business stakeholders. Section 3 specifies the requirements for
the product and development process. This section is intended for all stakeholders, especially the development team.

## 2. Product Overview

### 2.1 Product Functions

Summarize the major functions the product must perform or must let the user perform. Details will be provided in Section 3, so only a high level summary (such as a bullet list) is needed here. Organize the functions to make them understandable to any reader of the SRS. A picture of the major groups of related requirements and how they relate, such as a top level data flow diagram or object class diagram, is often effective.

### 2.2 Product Constraints

This subsection should provide a general description of any other items that will limit the developer’s options. These may include:  

### 2.3 User Characteristics

Identify the various user classes that you anticipate will use this product. User classes may be differentiated based on frequency of use, subset of product functions used, technical expertise, security or privilege levels, educational level, or experience. Describe the pertinent characteristics of each user class. Certain requirements may pertain only to certain user classes. Distinguish the most important user classes for this product from those who are less important to satisfy.

### 2.4 Assumptions and Dependencies

List any assumed factors (as opposed to known facts) that could affect the requirements stated in the SRS. These could include third-party or commercial components that you plan to use, issues around the development or operating environment, or constraints. The project could be affected if these assumptions are incorrect, are not shared, or change. Also identify any dependencies the project has on external factors, such as software components that you intend to reuse from another project, unless they are already documented elsewhere (for example, in the vision and scope document or the project plan).

## 3. Requirements

### 3.1 Functional Requirements

#### 3.1.1 User Interfaces

Web pages using HTML, CSS, and TypeScript.

#### 3.1.2 Hardware Interfaces

Devices that have web browser support.

#### 3.1.3 Software Interfaces

* Java JDK 21
* PostgreSQL 17
* SpringBoot 3.4.5
* TypeScript 5.8.3
* React 19.1.0

### 3.2 Non Functional Requirements 

#### 3.2.1 Performance

1. BrainDump will require less than 200 MB of working memory and less than 1 GB of persistent storage.
2. Application will support interactive response times of less than 10 seconds round trip.
3. New users will be able to create and publish a basic article without prior instruction.

#### 3.2.2 Security

4. Username and password authentication will be performed for any action that modifies data.

#### 3.2.3 Reliability

5. The application will possess 100% unit test coverage for all functionality.

#### 3.2.4 Availability

6. BrainDump will be available 24 hours a day, 7 days a week. Unless maintenence windows are explicitly booked with prior user notification. 

#### 3.2.5 Compliance

7. No personal data beyond email address will be maintained by the application.
8. No financial data will be retained by the application.
9. Users will be warned not to publish personal data within articles.

#### 3.2.6 Cost

10. No costs are permitted beyond the unpaid labor provided by the contributors.

#### 3.2.7 Deadline

11. The final product and associated documentation will be delivered on June 18th.
