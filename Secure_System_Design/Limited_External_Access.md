# Limited External Access

Most HPC systems that users are likely to have access to have some form of limited external access, including university, academic, national labs and commercial systems amongst others. These restrictions might include:

* No direct connection to the internet from the compute
nodes.
* No direct connection to the internet from the login nodes.
* Disabled outgoing ssh connections from the compute
nodes.
* Disabled outgoing ssh connections from the login nodes.
* Disabled ssh connections on the compute nodes.
* No access for machines with dynamic IP addresses allowed, end-users can only access from a static IP address, which has are often added to the allowed list.

Most HPC centers will allow some form of internet access on their login nodes to help facilitate data transfer from internet connected server, such as git repositories, Python, R, Julia and Jupyter etc. While some data centers do not allow direct internet connections, for example, the SuperMUC-NG cluster at LRZ does allow a direct internet to the system and endusers have to use other mechanisms to transfer data, for example, using reverse ssh tunneling.

Since the ssh exploited of early 2020 that effected a large number of HPC centers in Europe, where malicious actors used non password protected ssh keys stored in users home directory to connect to other HPC systems and gain privileged access (root). As a result of this action many European data centers have disabled outgoing ssh connections from their systems.
