# User Story for Legacy File Upload History

**As a** legacy wallet administrator,
**I want** to view the upload history of legacy wallet files via the application portal, 
**so that** I can effectively manage the members of my cooperative and agency.

#### **Who**:  
- **User**: A legacy wallet administrator responsible for managing and reviewing uploaded legacy files.

#### **What**:  
- **Feature**: Provide a feature that allows the administrator to view the history of legacy file uploads through the application portal.

#### **Why**:  
- **Value**: This functionality helps the administrator track file uploads, ensuring that member management and record-keeping are efficient and up to date.

---

### **Acceptance Criteria**

#### **Scenario 1: Legacy File Upload History**
- **Given** the user is logged in to the application portal,
- **And** the user has the required access permissions,
- **And** the user is on the "Associate Management" page within the wallet management section,
- **And** the user is in the "Upload Spreadsheet" tab,
- **When** the user accesses the page,
- **Then** the user should see a history section displaying file upload records from the past 90 days, with details as specified in the Figma design (link provided below).


#### **Scenario 2: Download Legacy File Upload History**
- **Given** the user is logged in to the application portal,
- **And** the user has the required access permissions,
- **And** the user is on the "Associate Management" page within the wallet management section,
- **And** the user is in the "Upload Spreadsheet" tab,
- **And** the user is viewing the file upload history section,
- **When** the user clicks the three-dot button at the end of any line in the upload history,
- **Then** a download button should appear, and when clicked, the user should be able to download the corresponding upload history file.

---

### **Business Rules**
- **Scenario 1**: The file upload history section must include the following columns:
  - The columns should be populated with data fetched from the relevant service.
  - The history should only display records for entities the user has access to.
  - The upload history should be paginated, showing 10 records per page.
  
- **Scenario 2**: The three-dot button at the end of each history entry should allow the user to download the corresponding uploaded file:
  - A request should be made to the service to fetch the relevant file according to pagination.
  - Only users with the appropriate access permissions will be able to download files.

---

### **Resources**
- **Figma**: [Link to Figma](#)
- **Swagger**: [Link to Swagger](#)
- **Documentation (Wiki)**: [Link to Wiki](#)
