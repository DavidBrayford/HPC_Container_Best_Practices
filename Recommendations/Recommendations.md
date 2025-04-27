# Reccommendations

In this section we provide some recommendations for deploying containerized workflows on secure HPC systems.

* Build containers from recipes using Dockerfiles, as they are relatively easy to create, replicate, modify and verify.
  
* Container build recipes are easy to produce workflow and system specific containers.
  
* Recipes provide the ability to generate performance portable containers based on the specific hardware & software setup of the system.
  
* Only a small amount of space is required for storing recipes in the form of are text files (Dockerfiles).
  
* If possible, use existing verified Dockerfiles to create new Dockerfiles for your containerized workflow image.
  
* Bring together the key stakeholders to formulate a container strategy and container recipes for your organization.
  
* Provide a standard recipe format and a consistent method for the generation of Dockerfiles and images across all groups and supported systems within the organization.
  
* Ensure that the Dockerfiles are compliant and consistent with different container technologies, which can be potentially used.
  
* Simplify the process of creating Dockerfiles and container images.
  
* Generate container images that have small memory footprints (minimal container image size).
  
* Work with HPC container developers to provide a simplified build and deployment methods
  
* Avoid installing anything into directory inside the container that the HPC container runtime mounts from the host.
