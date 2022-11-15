Link to the stock-predictor repo: 

https://github.com/yinghu-math/stock-predictor


**Q1** What does it mean to create a Docker image and why do we use Docker images?

Different machines have different architectures, operating systems, etc., so one application that runs on one machine may not run on another machine out-of-box. Setting up the environment for every machine and every application is a huge pain.  

To solve this problem, one can build a docker image that contains all the necessary contexts for the application and share the image instead of just the application. 
On the new platform, Docker can create a container according to the contents inside the image, within which the application can run properly.  

**Q2** Please explain what is the difference from a Container vs a Virtual Machine?

The virtual machine contains an entire operating system, and it virtualizes the file systems, the hardware etc. Virtual machines are stand-alone computers running on top of the host OS. You can run any application on a virtual machine. It's powerful and versatile but slow. 

The container itself doesn't contain an operating system; rather, it is more like a process running on top of the host OS. One container usually only contains one application or service. As a result, it's light and fast to boot up. 

**Q3** What are 5 examples of container orchestration tools (please list tools)?

**Ans:** Kubernetes, Openshift,  Docker Swarm, Nomad, Racher, Google Container Engine etc. 

**Q4** How does a Docker image differ from a Docker container?

**Ans**: When we `docker run` a Docker image, Docker creates a container using the instruction and contexts in an image. The container contains the applications and the necessary packages for the applications. 