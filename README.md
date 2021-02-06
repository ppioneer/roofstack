# roofstack


Rest Service to process json and create Account, Contact and Opportunities if they are not exist in System


1. Setps to Configure your Postman: 
	1. Download the Roofstock.postman_collection_v2 from the repo
	2. Open Postman
	2. Check the Import Options
			a. Import the collections file which you downloaded(Step 1)
	3. Select the Roofstack folder on left hand side
			a. Click on "oAuth_Login" request tab
			b. Hit the Send request button
			c. Once you get the response code as 200, copy the "access_token" key's value
	4. To make REST call to dev org for the service, Open "Assignment Validation" request tab	
			a. Past the the access_token copied from step 3.c to Headers of the current request. eg. ghjkjhg5678987fghjklkjhg
			b. Replace the old access token value in the Authoriziation header key value (After Bearer << step 3.c value>>)
					Example : Your Authoriation header value will be like this Authorization: Bearer ghjkjhg5678987fghjklkjhg	
			c. Now provide your json request body in the Body tab (type  = choose raw of type JSON(applicaiton.json))
	5. Now hit send request
			a. If the request is success(Status code = 200) ==> Records created/updated successfully
			b. If the request is failed (status code = 400) ==> for any errors

2. Download the clasess zip file to your local and deploy to your sandbox to validate/Testing

Demo Video link : https://drive.google.com/file/d/10GAckdFiE_lWjeXcRpg2p9c_Jfp0IJFx/view?usp=sharing 
Note: Please download the demo to view 

	
***	EOF ***
	
