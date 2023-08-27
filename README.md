# Kubernetes
Tutorial on what is Kubernetes and different commands to try. If you like this, feel free to fork. Happy Coding :)

**`Traditional Deployment Era`**: Organizations ran applications on physical servers with no way to define resouce boundaries for applications in physical server causing resource allocation issues. Example: You have application A, B and C running on same physical server. Application A is taking most of the resources at some time and as a result B and C are underperforming. Solution: Run each application on different physical server. But this does not scale as resources are underutilized and needs to maintain many physical servers.

**`Virtualized Deployment Era`**: Allows to run multiple Virutal Machines (VMs) on a single Physical Server's CPU. Virtualization allows applications A, B and C to be isolated between 3 VMs and provides a level of security as info of one App cannot be accessed by another App. Allows better utilization of resources and better scalability since an app can be easily updated. A Physical Server becomes a cluster of disposable VMs (Each VM is full machine running all components including own guest OS on top of virtualized hardware). VMs run on top of an emulating software called hypervisor which sits between hardware and virtual machine. Hypervisor is responsible for managing sharing of physical resources into virtual machines.

**`Container Deployment Era`**: Similar to VMs but have relaxed isolation properties to share Operating System among apps. Containers share common OS that requies care and feeding for bug fixes and patches. They are more agile and portable than VMs. Since they are decoupled from the underlying infra they are portable across clouds and OS distributions.

**`Difference between VMs and Containers and when to pick which one:`**
1. Need to run apps on different OS - VMs since VMs can run on different OS. Appplications running in a container env share a single OS. In case of containers, level of abstraction is raised from running an OS on virtual hardware to running on an OS using logical resources.
2. VMs virtualize Computer System whereas VMs virtualize OS only.
3. Size - VMs are large, containers are light few MBs.
4. Security - VMs are more secure since they do not allow one application to access another application's data.
5. VMs are useful when we reuire all of OS resources to run various apps.
6. Containers are useful when you required to run apps using minimal servers.
7. Agile application creation and deployment: increased ease and efficiency of container image creation compared to VM image use.
8. Continuous development, integration, and deployment: provides for reliable and frequent container image build and deployment with quick and efficient rollbacks (due to image immutability).
9. Dev and Ops separation of concerns: create application container images at build/release time rather than deployment time, thereby decoupling applications from infrastructure.
10. Environmental consistency across development, testing, and production: runs the same on a laptop as it does in the cloud.
11. Environmental consistency across development, testing, and production: runs the same on a laptop as it does in the cloud.




<img width="479" alt="image" src="https://github.com/poornimac1/Kubernetes/assets/9400009/146c10b8-8b77-431a-844d-dcaca6f0606a">

