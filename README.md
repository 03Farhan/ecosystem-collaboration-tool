## Welcome to Ecoystem Collaboration Tool.

An IBM Cloud account is required to run this webapp. After creating an account follow these instructions in order to create your Watson Collection and enter the information to access the Collection in the template.env file located in "./backend".

1. Login to your account and click on "Create resource".

![dashboard](./documentation/dashboard.png)

2. Type "Watson Discovery" into the search field and click on Watson Discovery. This will redirect you to a page where you can create a new free Watson Discovery Instance.

![create resource](./documentation/create-resource.png)

3. Fill out the fields to create the Watson Discovery Instance and then open the sidebar and click on "Resource List".

![sidebar](./documentation/sidebar.png)

4. Click on the new the new instance that you have created under the "Services" tab.

![resource list](./documentation/resource-list.png)

5. Copy the API Key and paste it to replace "<api_key>" in the template.env file and then copy the URL and paste it to replace "<service_url>" in the template.env file. Click "Launch Discovery".

![instance overview](./documentation/instance-overview.png)

6. Click on "Upload your own data" and enter a collection name (e.g. "Ecosystem Collaboration Tool") and then click "Create".

![create collection](./documentation/create-collection.png)

7. Once the collection has been made, click the API button near the top right and copy the "Collection ID" and "Environment ID" and paste it to replace the "<collection_id>" and "<environment_id>" respectively.

![collection API](./documentation/collection-api.png)

8. Rename the template.env file to ".env".

Now that Watson Discovery is setup, Docker is required to run this project and will eliminate the need to install dependencies onto your machine. Once Docker is installed and running, ensure that ports 3000 and 9000 are not being used by other programs. Now simply open terminal in this directory and run "docker-compose up" to start the webapp. Navigate to localhost:3000 on a browser and enjoy!
