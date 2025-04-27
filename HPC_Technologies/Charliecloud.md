# Charliecloud

Charliecloud [] was developed at LANL to be a lightweight open source UDSS implementation based on the Linux user namespace for HPC sites with strict security requirements. It uses Docker to build the HPC container image, shell scripts to unpack the image to an appropriate location and a C program to activate the image and run user code within the image.

In these secure environments, Charliecloud’s distinct advantage is the usage of the newly introduced user namespace to support non-privileged launch of containerized applications. The user namespace is an unprivileged namespace and within the user namespace, all other privileged namespaces are created without the requirement of root privileges, which means that a containerized application can be laun
