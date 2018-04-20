# Demos
Many demos and methods for delivering the demos are available.  Below is a recommended starting point and stratified list of demos based on complexity.

Environment Recommendations
-------------

Depending on the complexity of your demos you will need to assess the corresponding environment you will need to fully demonstrate the capabilities of OpenShift.  Below are the most commond and recommended ways for building/using OpenShift installs.

1) [Red Hat Product Demo System -- RHPDS](http://rhpds.redhat.com) -- This location has many pre-built demos that are excellent for customer demos.  These demos run on AWS and I have encountered more than one customer that blocks all AWS IP's so be pre-prepared to have alternative demos ready or alternative routes to the demo, i.e., hotpots, etc.

2) [CDK -- Container Development Kit](http://developers.redhat.com/products/cdk/overview/) 
	* Best for localized demos that don't require extensive resources or infracture demos like clustering, etc.

3) [oc cluster up](scripts/all-in-one-aws-template?raw=true)
	* Typically installed as an "all-in-one" deployment and when leveraging the Origin client tools can demonstrate the latest releases.  The steps for installing are itemized in this script.

4) [Reference Environments](https://github.com/openshift/openshift-ansible-contrib/tree/master/reference-architecture) 
	* These are ideal for demonstrating complex demos with larger resources and ideal for infrastructure related demos where you need show how to evict pods, add nodes, etc.


Best Practices
------------

* For the more advanced demos it is usually advisable to fork the demos to your local git repo so you can modify and interact with the source code.
	* Level 3 (Complex) -- best used on environments that have larger resources that can accommodate the Dev-Prod functionality.  This [link](https://github.com/jbossdemocentral/coolstore-microservice/tree/1.2.x/openshift/scripts) defines your deployment options.
		* [Coolstore Demo](https://github.com/jbossdemocentral/coolstore-microservice/) -- This is an example demo showing a retail store consisting of several microservices based on Red Hat OpenShift Application Runtimes -- RHOAR (Spring Boot, WildFly Swarm, Vert.x, JBoss EAP and Node.js) deployed to OpenShift.
![Cool Store Microservice Demo -- Architecture Diagram](docs/images/coolstore-arch-diagram.png?raw=true "Cool Store Microservice Demo -- Architecture Diagram")
	
	* Level 2 (Mid Level) -- best used to showcase deployment options, i.e., BlueGreen, Canary, etc., to both developers and operations.
		* [BlueGreen](https://github.com/sclorg/nodejs-ex) -- This is an example demo that imports a yaml template file instead of the typical bundled templates to show developers additional flexibility for creating solutions and embedding Jenkins pipelines with their applications.
![BlueGreen -- Jenkins pipeline demo](docs/images/bluegreen-arch.png?raw=true "BlueGreen -- Jenkins pipeline demo")


	* Level 1 (Entry Level)
		* These are intended to quickly show a customer a deployment leveraging core templates and images with associated quick start demos that are included with OpenShift.

# Workshops
The primary location for workshops should be this git repo authored by the [Tiger Team](https://github.com/RedHatWorkshops/openshiftv3-workshop/).

Environment Recommendations
-------------
* One of the main problems with workshops/labs is getting the client tools to the customers and installed on their computers prior to the engagement.  This [link](https://github.com/RedHatWorkshops/openshiftv3-workshop/blob/master/0-Setting-up-client-tools.adoc#setting-up-client-tools) is to the first lab that has details and links on obtaining and installing the oc client tools needed for all of the labs and workshopts.  It is highly recommended that you share this with customers prior to the workshops if possilbe to try and minimize the time spent installing the oc tools.
