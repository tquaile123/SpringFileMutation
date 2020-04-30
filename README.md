# SpringFileMutation
Build a Spring Boot 2+ Service using Maven that consumes a xml file and returns a response containing information about the individual entries in the bulk file.

## Information 
The xml file attatched is broken into individual sets of information identified by the `</>`tag. 

The xpaths to build the responses can be found bellow : 
Policy Number - 
Customer Name - 
Policy Type - 
Total Premium - 
Vehicle Make -
Vehicle Model - 
Vehicle Premium - 
Vehicle Collision Deductible - 
Driver Name - 
Driver Ahe -


## Response Format 
The response should contain an array of the following information extracted from the file and a count of the number of entries: 
```json
{
"policyNumber": String,
"customerName": String,
"PolicyType": String,
"totalPremium": Float,
"vehichles": [{
"make" : String,
"model": string,
"premium": Float,
"collisionDeductible": Float
}...],
"drivers" : [{
"driverName": String,
"age": Integer
}...]
```
