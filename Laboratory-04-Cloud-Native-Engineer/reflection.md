# Mission Reflection

This laboratory helped me understand the fundamentals of Docker and cloud-native technologies. One of the most noticeable differences between Docker containers and Virtual Machines is the boot time and setup process. Installing an operating system on a Virtual Machine can take several minutes because a complete guest operating system must be installed and configured. In contrast, a Docker container can start within seconds because it shares the host operating system kernel and only includes the application and its required dependencies.

Port mapping using the `-p 8080:80` option is necessary because containers operate in an isolated environment. The Nginx web server listens on port 80 inside the container, while port 8080 on the host machine acts as the access point. Port mapping creates a connection between the host and the container, allowing users to access the web server through a browser.

When the `docker rm` command is used, the container is permanently removed from the system. Any data stored only inside that container is also deleted. This is why persistent data should be stored in Docker volumes or external storage if it needs to be retained after the container is removed.

Containerization has significantly changed the way software developers and IT operations teams work together. Developers can package applications with all required dependencies into containers, ensuring consistency across different environments. Operations teams can deploy the same containers without worrying about configuration differences. This supports DevOps practices by improving collaboration, reducing deployment issues, and increasing efficiency.

My GitHub portfolio is evolving as I complete more cloud computing laboratories and technical projects. Each repository demonstrates new skills, such as cloud infrastructure planning, multi-cloud research, and container management. By documenting my work and uploading evidence of completed activities, I am building a portfolio that showcases my growing knowledge in cloud computing, DevOps, and modern software development practices.
