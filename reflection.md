# Mission Reflection

This laboratory activity helped me understand how containerization works and why Docker is useful in cloud computing. Before performing the activity, I knew that Docker was used for containers, but I had less experience with actually deploying and managing one. Using the KillerCoda Playground allowed me to practice Docker commands and see the process in action.

First, the boot time and setup process of a Docker container is much faster than installing an operating system on a Virtual Machine. A Virtual Machine needs its own guest operating system and usually requires more resources and setup time. With Docker, I was able to download the Nginx image and start the web server using only a few commands.

Second, port mapping using `-p 8080:80` is necessary because it connects a port on the host machine to a port inside the container. In this activity, port 8080 on the host was connected to port 80 of the Nginx container. This allowed me to access the web server by using `http://localhost:8080`.

Third, using `docker rm` removes the container. Data stored only inside the container can be lost when the container is removed, which shows why persistent data needs appropriate storage when it must remain available.

Fourth, containerization can improve collaboration between software developers and IT operations teams. Developers can package an application and its dependencies into a container, while operations teams can deploy the same container in different environments. This can make deployment more consistent and efficient and supports the goals of DevOps.

Finally, my GitHub portfolio is gradually becoming a record of my cloud computing skills. My previous laboratory activities and this Docker activity show my progress from learning cloud infrastructure concepts to performing practical cloud-native operations. This laboratory gave me hands-on experience with Docker and container management.
