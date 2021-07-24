# EhealthProject
Project assignment  
The web api solution is built using ASP.NET Core MVC that has all CRUD opeartion in it using repository pattern.
I have not consider the database connection and azure services since it was not feasible to add these that would have make it more effective.

For sample purpose i have hard-coded one contact  which can be edited and found in repository class file (ContactRepository.cs)

Use fiddler to test the API's call here 
a) List all the data 
I have added sample data whenever you run the application it will create one contactId

Method: GET 
URL :  http://localhost:44282/api/Contact/

b) Add new contact 
Use fiddler tool to test the api call 
 
Method : POST  
URL : http://localhost:44282/api/Contact/Create/
Request body : 
{"firstName":"Lassy","lastName":"Emual","email":"lassy.emual@gmaill.com","phoneNumber":907899208,"status":"InActive"}

c) Upate the record 
Method : PUT
URL : http://localhost:44282/api/Contact/{"Provide the contactid}/
Request body : [{"contactId":"a82ba625-d864-463c-9930-84b845d17670","firstName":"Sam","lastName":"Billing","email":"sam.billing@hotmail.com","phoneNumber":98777729,"status":"InActive"}]

d) Delete the record
Method : Delete
URL : http://localhost:44282/api/Contact/{"Provide the contactid}/
Request body : Not required 
