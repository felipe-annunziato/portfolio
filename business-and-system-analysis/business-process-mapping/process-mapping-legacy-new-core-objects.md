# Business Process Mapping 📝

## Example: Legacy and New Core Data Integration

### Context:
In one of the significant projects I worked on, we had two customized Salesforce objects that received and processed information, one for the legacy core records and the other for the new core. However, this setup was limiting users and other teams from accessing and utilizing the data effectively, as the relationships between the objects were not well-integrated.

### Solution:
We conducted an analysis of the BranchUnit object within Financial Service Cloud, which was better suited for our needs. This led to a plan for unifying the structure of the objects.

#### **Steps Involved**:
1. **Current State Mapping (AS-IS)**:
   - As a person responsible for this redesign, I created a visual representation of the existing object structure in Figma, highlighting the limitations of the legacy and new core objects.
   
2. **Future State Mapping (TO-BE)**:
   - I redesigned the structure to unify the objects by using BranchUnit module objects as the default.
   
3. **Trigger Mapping**:
   - The team and I mapped out all the triggers involved with the objects and determined what changes were necessary.
   
4. **Integration with External Services**:
   - We identified external services (Kafka, APIs) that fed data into the objects and how they would interact with the new structure.
   
5. **Message Standardization**:
   - We defined the message formats to ensure smooth data transfer between systems.
   
6. **Field Mapping**:
   - We determined the necessary fields for the objects to work in the new structure.

This was a large-scale project, and while I did not directly oversee the final deployment, I was responsible for leading the mapping process and ensuring the execution of the redesign.
