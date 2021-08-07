# jmeter
https://university.blazemeter.com/

# Old Style
Download plugins from https://jmeter-plugins.org/
Unzip and place the files in ./lib/ext
Remember to quit and restart j-meter

# New Style
Options -->Plugins Manager
This available only after placing the plugins manager described in above method.

# J-meter
http://jmeter.apache.org/download_jmeter.cgi

# First Building Blocks
	1. Test Plan
		a. Enable the "Run the thread groups to run consecutively" to run them in sequence.
	2. Thread Groups
		a. Determine the # of virtual users (10)
		b. Ramp up in seconds (60)
		c. If there are multiple thread groups under test plan they get executed parallelly.
	3. Samplers
			i. HTTP Request
				1) www.demoblaze.com
				2) Method : GET
				3) Body
				4) Params
				5) Headers, etc
			ii. TCP Sampler
			iii. JDBC Request
			iv. SSH Command
	4. Timers
		a. Constant timers
			i. Delay : 300 milli seconds
		b. Uniform random timer
		c. Precise Through put timer
		d. Constant Through put timer,etc
	5. Assertions
		a. Response assertion
		b. Json assertion
		c. Xpath assertion
		d. Size assertion
		e. Bean shell assertion
		
	6. Pre/Post Processors
		a. Preprocessors to ex: to get data from DB before the sampler is run
		b. Post processor to extract data from post headers like session variables etc. so that they can be used further
	7. Listeners
		a. View Results Tree
			i. Load Time
			ii. Connect Time
			iii. Latency
			
		b. Summary Report
			i. Throughput : The number of requests that are processed per min or sec or hours.
			ii. Average : Average response time taken by all the sampler
		c. Aggregate Report
		d. Backend Listener
		
# Configuration Elements
	1. HTTP Request Defaults
		a. Holds the global variables like common hostname, parameters that can be used by subsequent requests  in the Thread Group.
	2. HTTP Header Manager
		a. Let's you add or override http headers.
	3. HTTP Cache Manager
		a. Is used to add caching functionalities.
	4. HTTP Cookie Manager
	5. DNS Cache Manager
	
# Logic Controllers
Serves as a storage device by grouping the samplers logically by pages/transactions(likes Actions in UFT)
	1. Simple Controller
	2. Transaction Controller

# Performance Metrics

# Using Test Record Template
	1. File-->Template-->Test Record Template
	2. Right click on Test Script Recorder and Enable
	3. Set up windows proxy to listen on 8080 ..if the application is to be on localhost.
		a. Start -->Internet Options-->Connections-->LAN Settings -->Address(localhost) and port 8080.
		b. Go to chrome --> Settings-->Security-->Manage Certificates-->Import the CA Certificate.
	4. Click Start to record.

# Concurrency Thread Group
# Ultimate Thread Group
# SetupThreadGroup
# TearDownThreadGroup

# JmeterFunctions
