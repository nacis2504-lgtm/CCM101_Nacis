# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's work easier because the configuration of different containers can be placed in one file. Instead of entering several commands one by one, the engineer can simply use `docker-compose up -d` to start the required services. This saves time and makes the deployment easier to repeat if the system needs to be deployed again.

An indentation error in a YAML file can cause the Compose file to become invalid. For example, using a Tab instead of Spaces can result in an error when Docker Compose tries to read the file. I learned that YAML is sensitive to spacing, so proper indentation is important when writing configuration files.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` are used to provide the information needed by the application and database. They help Nextcloud connect properly to the MariaDB container. Using variables also keeps the configuration organized and makes it easier to change settings without changing the whole configuration.

Deploying Nextcloud in just a few minutes was a good experience for me because I was able to see how quickly a cloud application can be set up using Docker Compose. At first, the configuration looked complicated, but after following the steps and running the commands, I was able to access Nextcloud through the browser. It made the deployment process feel more manageable.

Since Mission 1, my understanding of Cloud Computing has improved a lot. I first learned the basic concepts of cloud computing, and then I learned about virtualization, containers, Docker, storage, and cloud deployment. This mission helped me understand how these concepts can work together. I also learned that automation and proper configuration are important skills for a cloud engineer.
