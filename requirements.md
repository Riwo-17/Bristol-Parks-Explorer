# Requirements

## User Needs

### User stories
As a  Bristol resident, I want to be able to browse for details of parks and green spaces in bristol so that I can learn more about it before visiting.

As a Bristol resident, I want to filter parks and green spaces so that I can find locations that match my preferences.

As a resident, I want to be able to search for specific parks so that I can find it without scrolling through the entire directory.

### Actors
App User	A person who visits the website to browse, search and filter parks and green spaces.
Registered User	A user who has created an account and can access additional personalised features.
Administrator	A person responsible for managing the website and maintaining its information.


### Use Cases
TODO: Describe each use case (at least one per team member).
    Give each use case a unique ID, e.g. UC1, UC2, ...
    Summarise these using the use-case template below.

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
## 3. Use Cases

### UC1 – Search for Parks

| Field | Description |
|---|---|
| **Description** | Allows users to search for specific parks in Bristol. |
| **Actors** | App User, Registered User |
| **Assumptions** | Park records are available in the system. |
| **Steps** | 1. User opens the parks directory. 2. User enters a park name. 3. System searches the records. 4. System displays matching results. |
| **Variations** | If no matching parks are found, the system displays a message. |
| **Non-functional** | Search results should load promptly. |
| **Issues** | Search depends on the accuracy of park records. |

### UC2 – Filter Parks

| Field | Description |
|---|---|
| **Description** | Allows users to filter parks according to available categories or classifications. |
| **Actors** | App User, Registered User |
| **Assumptions** | Park records contain suitable category information. |
| **Steps** | 1. User opens the parks directory. 2. User selects a filter. 3. System applies the filter. 4. System displays matching parks. |
| **Variations** | If no parks match, the system displays a message. |
| **Non-functional** | Filters should be easy to understand and use. |
| **Issues** | Available filters depend on the dataset. |

### UC3 – Explore Park Details

| Field | Description |
|---|---|
| **Description** | Allows users to view available information about a selected park. |
| **Actors** | App User, Registered User |
| **Assumptions** | Park information is available in the system. |
| **Steps** | 1. User selects a park. 2. System retrieves its information. 3. System displays the park details. |
| **Variations** | If information is unavailable, the system displays a message. |
| **Non-functional** | Information should be clearly presented. |
| **Issues** | The details displayed depend on the available data. |

### UC4 – Save Park

| Field | Description |
|---|---|
| **Description** | Allows registered users to save parks to their personal favourites. |
| **Actors** | Registered User |
| **Assumptions** | The user is logged in and the selected park exists. |
| **Steps** | 1. User selects a park. 2. User clicks the save button. 3. System saves the park to their favourites. 4. System confirms that the park has been saved. |
| **Variations** | If the park is already saved, the system informs the user or allows them to remove it. |
| **Non-functional** | Saved parks should remain available when the user logs in again. |
| **Issues** | User accounts and a database are required. |

### UC5 – Manage Park Records

| Field | Description |
|---|---|
| **Description** | Allows administrators to add, update and delete park records. |
| **Actors** | Administrator |
| **Assumptions** | The administrator is authenticated and has permission to manage records. |
| **Steps** | 1. Administrator logs in. 2. Administrator accesses the management area. 3. Administrator selects a record to add, edit or delete. 4. System processes the changes. 5. System confirms the action. |
| **Variations** | If the information is invalid, the system displays an error message. |
| **Non-functional** | Administrative functions should be secure and reliable. |
| **Issues** | Administrator authentication and data validation are required. |
| -------------------------------------- | ------------------- |

TODO: Your Use-Case diagram should include all use-cases.

![Insert your Use-Case Diagram Here](images/use-case.png)
UseCase Diagram.asta

## Software Requirements Specification
### Functional requirements
## 4. Software Requirements Specification

### 4.1 Functional Requirements

| ID | Functional Requirement | Use Case |
|---|---|---|
| FR1 | The system shall allow users to search for parks by name. | UC1 |
| FR2 | The system shall display parks matching the user's search input. | UC1 |
| FR3 | The system shall display a message when no matching parks are found. | UC1 |
| FR4 | The system shall allow users to filter parks by available categories. | UC2 |
| FR5 | The system shall display parks matching the selected filters. | UC2 |
| FR6 | The system shall allow users to clear their selected filters. | UC2 |
| FR7 | The system shall allow users to select a park and view its available details. | UC3 |
| FR8 | The system shall display available information about the selected park. | UC3 |
| FR9 | The system shall allow registered users to save parks to their favourites. | UC4 |
| FR10 | The system shall allow registered users to view their saved parks. | UC4 |
| FR11 | The system shall allow registered users to remove parks from their favourites. | UC4 |
| FR12 | The system shall allow users to create an account and log in. | UC4 |
| FR13 | The system shall allow administrators to add new park records. | UC5 |
| FR14 | The system shall allow administrators to edit existing park records. | UC5 |
| FR15 | The system shall allow administrators to delete park records. | UC5 |


### Non-Functional Requirements
TODO: Consider one or more [quality attributes](https://en.wikipedia.org/wiki/ISO/IEC_9126) to suggest a small number of non-functional requirements.
Give each non-functional requirement a unique ID. e.g. NFR1, NFR2, ...

Indicate which UC the requirement comes from.
### 4.2 Non-Functional Requirements

| ID | Quality Attribute | Non-Functional Requirement | Use Case |
|---|---|---|---|
| NFR1 | Usability | The website shall provide clear navigation and understandable labels. | UC1–UC5 |
| NFR2 | Performance | Search and filter results shall load within 3 seconds under normal operating conditions. | UC1, UC2 |
| NFR3 | Security | The system shall protect registered users' account information and prevent unauthorised access to administrator features. | UC4, UC5 |
| NFR4 | Reliability | Saved parks shall remain associated with the correct registered user after logging out and back in. | UC4 |
| NFR5 | Compatibility | The website shall function correctly on current versions of Chrome, Edge and Firefox. | UC1–UC5 |
| NFR6 | Accessibility | The website shall support keyboard navigation and use readable text and sufficient colour contrast. | UC1–UC5 |
| NFR7 | Responsiveness | The website shall adapt its layout to desktop, tablet and mobile screen sizes. | UC1–UC5 |
