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
        ## SMALL
         - 1 vCPU, 1 core, 1GB RAM on private cloud
         - t2.micro on AWS public cloud
         - Web tier VM starts at 1 replica and can scale to a maximum of 2, all others services cannot scale.
         
         ## MEDIUM
         - 2vCPUs, 2 cores, 1GB RAM on private cloud
         - t2.micro on AWS public cloud
         - Web tier VM starts at 2 replicas and can scale to a maximum of 4, all others services cannot scale.
         
# for security, No VM resource parameters can be changed by the end user

 - After deployment, a developer can perform a database backup or a database restoral operation at any time
 - The database VM is a monolith and uses MySQL, latest version 8.x software
 - The database was hosted on the public cloud and allows database access from the public and private cloud web tier hosts
