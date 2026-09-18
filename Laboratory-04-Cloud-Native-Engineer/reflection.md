# Mission Reflection

  Docker containers typically offer faster startup times compared to Virtual Machines, as they utilize the host operating system's kernel rather than booting an entire guest operating system. During my laboratory session, I successfully pulled the Nginx image and launched it as a container using just a few Docker commands, whereas setting up a Virtual Machine would typically involve more extensive configuration, including resource allocation and operating system installation.

   The `-p 8080:80` command facilitates the mapping of port 8080 on the host to port 80 within the Nginx container. While Nginx operates on port 80 internally, I accessed it externally via port 8080 on the host. This port mapping enabled me to effectively test the web server using the command `curl http://localhost:8080`.

   The command `docker rm nginx-server` is utilized to delete a container once it has been stopped. This action removes the container's writable layer and any specific data associated with it, while the Nginx Docker image remains intact unless explicitly deleted. This experience highlighted the transient nature of containers, which can be created and removed independently of their underlying images.

   Containerization enhances collaboration between development and IT operations teams by ensuring a uniform application environment. Developers can encapsulate an application along with its necessary dependencies, allowing operations teams to deploy the same container across various environments. This consistency streamlines processes related to testing, deployment, and troubleshooting.

   My GitHub portfolio is becoming increasingly organized as I consolidate each Cloud Computing laboratory into a single repository. Laboratory 4 contributed practical experience with Docker and containerization, covering aspects such as deployment, container lifecycle management, and technical documentation. By keeping commands, screenshots, Markdown files, and reflections in one place, I can more easily track my progress and showcase the skills I have acquired.
