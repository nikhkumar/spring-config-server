# spring-config-server
Example for Spring Cloud Config Server

Spring Cloud Config is Spring's client/server approach for storing and serving distributed configurations across multiple applications and environments.

The Git-backed configuration API provided by our server can be queried using the following paths:

	/{application}/{profile}[/{label}]
	/{application}-{profile}.yml
	/{label}/{application}-{profile}.yml
	/{application}-{profile}.properties
	/{label}/{application}-{profile}.properties

In which the 	

	{label} 	placeholder refers to a Git branch, 
	{application} 	to the client's application name and the 
	{profile} 	to the client's current active application profile

http://localhost:8001/client-config/development

	{	
		"name":"client-config",
		"profiles":["development"],
		"label":null,
		"version":"b724660defe13761c234032673751adff65fb582",
		"state":null,
		"propertySources":[]
	}


http://localhost:8001/client-config/production
