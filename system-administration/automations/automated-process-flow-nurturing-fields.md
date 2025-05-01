# Automated Process Example: Campaign Data Update

## Problem:
In a Salesforce setup, the campaign data wasn't being updated automatically in the related Contact records, causing inconsistencies in the nurturing fields, which are used to guide the donor's journey through Account Engagement. 

## Solution:
I created a Record-Triggered Flow to automate the process of updating Contact fields based on the Campaign they are associated with. The Flow checks the status of the Campaign (whether it's ongoing or completed), and depending on the conditions, updates or clears the Contact fields accordingly:
1. If the Campaign is ongoing and is the most recent one the Contact is associated with, the fields are updated.
2. If the Campaign is completed and is the most recent, the fields are cleared.
3. If neither condition is met, the Flow stops.
