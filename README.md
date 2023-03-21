## MyDevilopments

[Integration patterns](#integration-patterns-)

## Integration patterns [^](#mydevilopments)

## 1. Request & Reply [^](#integration-patterns-)

- Salesforce invokes a process on a remote system, waits for the completion of that process, and then tracks the state based on the response from the remote system.

### 1.1. Client requirement [^](#request-&-reply-)

- A utility company uses Salesforce and has a separate system that contains customer billing information. 
- They want to display the billing history for a customer account without storing that data in Salesforce. 
- They have an existing web service that returns a list of bills and the details for a given account, but can’t display this data in a browser.

### 1.2. Analisis [^](#request-&-reply-)

- When: On click button "Display billing history" on record layout of entity Account
- What: Salesforce should perform a synchronous callout to a middleware and rerender page with Billing History records
- Considerations: No DML can be performed on any of the systems. Operation can't be done from sites

### 1.3. REST [^](#request-&-reply-)

- 

### 1.4. SOAP [^](#request-&-reply-)

-

