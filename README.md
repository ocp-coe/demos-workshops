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

For the more advanced demos it is usually advisable to fork the demos to your local git repo so you can modify and interact with the source code.
	* Level 3 -- Complex
		* Coolstore Demo -- 

Level 1
These are intended to quickly show a customer a deployment leveraging core templates and images with associated quick start demos

