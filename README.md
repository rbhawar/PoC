# PoC


Steps/commands to execute the PoC:

Note: After extracting the files from archive, please ensure to change the permissions (to 755) and ownership of the files, so that it can execute on the system.

Step 1: cd Rupali-PoC/apache-poc
Step 2: Build apache poc docker image using below command. 
	docker build -t rupaliapachepoc1 .
Step 3: Deploy the container
	docker run -it -d -p 80:80 rupaliapachepoc1


Step 4: cd Rupali-PoC/tomcat-poc
Step 5: Build tomcat poc docker image using below command. 
	docker build -t rupalitomcatpoc1 .
Step 6: Deploy the container
	docker run -it -d -p 8084:8080 rupalitomcatpoc1

Step 7: Open the browser on your system and paste the link http://localhost:80
Step 8: Mention the username and password as ruser2/ruser2


You shall be able to see the Hello world application


Note: For now the above commands will deploy the application on the localhost. We can deploy it on multiple hosts by using Ansible play by mentioning the multiple hosts in the inventory.


