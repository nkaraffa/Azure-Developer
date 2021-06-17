# Azure Developer

### (AZ-204): What I learned about developing applications in Microsoft Azure 
________________________
## Content

**Creating Azure App Service Web Apps**

	• App Service Plans
		• App Service plans can be logically group apps within a subscription:
			§ Characteristics such as features, capacity, and tiers are shared among the website instance in the group.
			§ The App Service plan is the unit of billing in most cases.
		• Multiple App Service plans can exist in a single Resource Group and multiple apps can exist in a single App Service plan.
		
	• Authentication and authorization
		• Built-in authentication and authorization support:
			§ No extra code required to make use of these features
		• User claims are made available to code:
			§ If you wish to enhance the authentication support, you can use your existing code with popular identity frameworks:
				□ ASP.NET Identity
				□ Server variables
		• Built-in token store

	• Azure App Service Hybrid Connections
		• Enables access to resources in other networks

	• Azure App Service Local Cache
		• Provides a write-but-discard cache of your content
		• Created asynchronously when site is started
		• Automatically serves content once the cache is ready
                • Faster than reading content from Azure Storage directly on each client request
		
	• App Service on Linux
		• Why Linux?
			§ Many applications stacks are optimized for Linux:
				□ Ruby/Rails, PHP, Node, and others
				□ Often, better tools are available on Linux for these stacks
			§ New and upcoming frameworks are built for Linux first and then Windows
			§ Portability of Docker containers
			§ Linux is at the forefront of innovations in nano and microservice architecture

	• OS & runtime patching
		• OS and application stack are managed by Azure on your behalf
		• Monthly OS patching:
			§ Physical servers
			§ Guest virtual machines
		• Stable versions of application runtimes are periodically added to App Services:
			§ Some are installed side-by-side, while others replace existing versions
			§ You can manually migrate from one application runtime to another
			


**Implement Azure Functions**

	• Azure Functions Overview
		• What can Azure Functions do?
			§ Run code based in HTTP requests
			§ Schedule code to run at predefined times
			§ Process new and modified
				□ Azure Cosmos DB documents
				□ Azure Storage blobs
				□ Azure Queue storage messages
			§ Respond to Azure Event Grid events by using subscriptions and filters
			§ Respond to high volumes of Azure Event Hubs events
			§ Respond to Azure Service Bus queue and topic messages
		• Azure Functions
			§ Solution for running small pieces of code, or functions, in the cloud:
						

		• Scale and Hosting
			§ You can choose between three types of plans:
				□ Consumption
					® Instances are dynamically instanced and you are charged based on compute time
				□ Premium
					® Instances of the Azure Functions host are added and removed based on the number of incoming events just like the Consumption plan, but provides additional features like: VNet connectivity; unlimited execution duration; and more predictable pricing
				□ App Service Plan
					® Traditional App Services model used with Web Apps, API Apps, and Mobile Apps
			§ The type of plan controls:
				□ How host instances are scaled out
				□ The resources that are available to each host
		• Bindings
			§ Declarative way to connect to data from your code:
				□ Connect to services without writing plumbing code
				□ Service credentials are not stored in code
				□ Bindings are optional
			§ Function can have multiple input and output bindings
			§ Output bindings can send data to Azure services such as:
				□ Storage
				□ Azure Cosmos DB
				□ Service Bus
					

		• Best Practices
			§ Avoid long-running functions
			§ Use queues for cross-function communication
			§ Write stateless functions
			§ Code defensively
			
	• Developing Azure Functions
		• Durable Functions
					

			§ Durable Function Methods
				□ Fan-out/Fan-in
				□ Async HTTP APIs
				□ Monitoring
				□ Human Interaction


**Develop solutions that use blob storage**

**Develop solutions that use Cosmos DB Storage**

**Implement IaaS Solution**

**Implement user authentication and authorization**
          
________________________
## Links

          o https://docs.microsoft.com/en-us/learn/certifications/exams/az-204
          o https://www.measureup.com/#dashboard.php
