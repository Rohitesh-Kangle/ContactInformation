There are two module/Project.

1. Web api project which helps us to interact with DB.

  a) Here I have used sql server as database and name of database is InfoDB.mdf which contains one table CustomerInformation.
  
  b)  CustomerInformation Table Info
  
      i)  Customer ID which is identity column
      ii)  FirstName which can accept 50 character
     iii)  LastName which can accept 50 character    
      iv)  Email which can accept 50 character
       v)  Phone number which can accept 10 charterer 
      vi)  status which is boolean to maintain if customer is active or inactive.
	 
  c) For communication between database and webpi I have used EntityFramework Database approach.

2. Asp.net MVC project which communicates with web api to perform operation.

   a) In this project, there are four minor module 
   
      i)  List customer details 
     ii)  Add customer details 
    iii)  Edit customer details 
     iv)  Delete customer details 
	  
   b) All this is done in Asp.net mvc
   

To Execute application please download both the application.
1. Open both the project with Visual studio.
2. Framework 4.5 is used to develop this project.
3. Run the web api project and copy url form browser.
4. Open the Webconfig of mvc project and search for key "WebApiUrl" and add url of your web api running project.
     E.g  <add key="WebApiUrl" value="http://localhost:55029/"/>
5. Once this is done run your mvc project.
6. Now you can use this application.

Pre-requites:
visual studio, framework and sql server installed.

Note:
if possible run both application with administrator rights.
