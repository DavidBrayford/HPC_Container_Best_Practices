# HPC Container Technologies

In this section we introduce some of the related technologies, which are commonly used to deploy containers on HPC systems.

## User Defined Software Stack

With the increasing demand on more flexible execution models from researchers the standard methods to offer software on HPC systems (i.e. predefined modules with specific software packages) becomes impractical. User Defined Software Stacks (UDSS) as defined by Priedhorsky et al. [R. Priedhorsky and T. Randles, “Charliecloud: unprivileged containers for user-defined software stacks in hpc,” in Proceedings of the International Conference for High Performance Computing, Networking, Storage and Analysis, ser. SC ’17. New York, NY, USA: Association for Computing Machinery, 2017. [Online]. Available: https://doi.org/10.1145/3126908.3126925] combined with the recently introduced user namespaces in Linux offer a solution to how those can be realized in the form of containers without sacrificing security of the HPC cluster.

The UDSS concept helps to deal with problems such as handling dependencies, frequent software updates and support of other Linux environments. User namespaces available in Linux, since Linux Kernel 3.8, allow the execution of privileged operations without escalating permissions up to root. No child processes do not have control over their parent processes. Mappings for UIDs and GIDs between parent and children processes make sure that operations are executing in a safe way by using the original ID of the end-user.
