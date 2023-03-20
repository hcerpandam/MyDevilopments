## MyDevilopments

[Integration patterns](#integration-patterns-)

## Integration patterns [^](#mydevilopments)

## 1. Request & Reply [^](#integration-patterns-)

### 1.1. Client requirement

- A utility company uses Salesforce and has a separate system that contains customer billing information. 
- They want to display the billing history for a customer account without storing that data in Salesforce. 
- They have an existing web service that returns a list of bills and the details for a given account, but can’t display this data in a browser.

### 1.2. Analisis

- When: On click button "Display billing history" on record layout of entity Account
- What: Salesforce should perform a synchronous callout to a middleware and rerender page with Billing History records
- Considerations: No DML can be performed on any of the systems

### 1.3. REST

- 

### 1.4. SOAP

-

