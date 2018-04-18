# Demos
Many demos and methods for delivering the demos are available.  Below is a recommended starting point and stratified list of demos based on complexity.

Environment Recommendations
-------------

Depending on the complexity of your demos you will need to assess the corresponding environment you will need to fully demonstrate the capabilities of OpenShift.  Below are the most commond and recommended ways for building/using OpenShift installs.

1) [CDK -- Container Development Kit](http://developers.redhat.com/products/cdk/overview/) 
	* Best for localized demos that don't require extensive resources or infracture demos like clustering, etc.

2) [oc cluster up](scripts/all-in-one-aws-template?raw=true)
	* Typically installed as an "all-in-one" deployment and when leveraging the Origin client tools can demonstrate the latest releases.  The steps for installing are itemized in this script.

3) [Reference Environments](https://github.com/openshift/openshift-ansible-contrib/tree/master/reference-architecture) 
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
		* These are intended to quickly show a customer a deployment leveraging core templates and images with associated quick start demos

