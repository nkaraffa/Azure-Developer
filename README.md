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

**Develop solutions that use blob storage**

**Develop solutions that use Cosmos DB Storage**

**Implement IaaS Solution**

**Implement user authentication and authorization**
          
________________________
## Links

          o https://docs.microsoft.com/en-us/learn/certifications/exams/az-204
          o https://www.measureup.com/#dashboard.php
