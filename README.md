# Hybrid-Cloud-Saas-Three-Tier-Web_App
The three tiers of the web application are:

_a load balancer_
_a web server_
_and a database server_

- All private Cloud VMs were built with CentOS 8 cloud image for located in the CentOS image repository (currently CentOS-8-GenericCloud-8.2.2004- 20200611.2.x86_64.qcow2)
- AWS Linux free tier option Red Hat Enterprise Linux 8 (HVM), SSD Volume Type were used for public instances
- The load balancer uses HAProxy software and was hosted on the private cloud
- The web tier uses Apache web server both on the private and the public cloud platforms
- There are two deployment a SMALL and a MEDIUM
        
