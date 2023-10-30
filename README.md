# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/7558cb49-4f3c-45f1-be2a-eaac3769f501)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/8efe69de-4205-40bb-81bf-acc1b4efcad2)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/b7b667de-949c-46c3-a84f-3c9e8575786d)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/0cde58e7-9cd1-4654-bb7c-ae9d0233a6db)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



## Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/2bc92ddb-f0df-412e-8f71-e3d450c4d9a6)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.

Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 
![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/3fe5fa31-1f68-47f3-aadd-a7bec0040a8f)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/b32081fa-a6c1-4c26-8a17-67b23b00cecc)

Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 
![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/56047cb1-407c-42e3-9faf-b3fee70b099f)


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/c86bfe35-02fb-408a-960c-6d41edc8a410)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/a7413e07-b995-44b8-8af9-9dbdba2c4e98)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/d8dde606-373d-4641-965c-fc5d6809f5a3)

Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
![image](https://github.com/varshithathirumalachari/Ex-04_RESTful_Web_Services/assets/131793193/ebc29fc8-87e2-4b45-8964-b84e3e0c95cd)


## Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
