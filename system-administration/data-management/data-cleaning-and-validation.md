# Data Management Example: Deduplication and Cleanup

## Problem 1: Duplicate Records in Salesforce
During the migration of customers from two system cores (legacy and new) into Salesforce, a process failure led to both old and new records being created. This caused confusion among users and polluted the database.

## Solution:
I wrote a SOQL query to identify and delete over 130K duplicate records in Salesforce, ensuring the database was cleaned up. The deduplication helped improve data integrity and user experience.

---

## Problem 2: Data Cleanup for Prospect List
At a charity where I worked, we reached the limit for mailable prospects in Salesforce's Account Engagement. We needed to reduce the number of prospects.

## Solution:
I performed an export of the prospect data, applied filters defined by the manager, and imported a list of prospects that needed to be archived. This cleanup allowed the charity to remain within the system's limits and improved email campaign efficiency.
