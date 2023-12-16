# Learning-Docker

## Basic

Certainly! Let's provide a more detailed explanation and purpose for each of the Docker commands and concepts you've mentioned:

### Docker Commands:

1. **`docker --version`**

   - **Explanation:** This command is used to check the version of Docker installed on your system.
   - **Purpose:** Verifying the installed Docker version is essential to ensure compatibility with Docker-related tasks and to identify potential issues related to version mismatches.

2. **`docker version --format '{{.Server.Version}}'`**

   - **Explanation:** Retrieves and displays the Docker server version in a specified format.
   - **Purpose:** Useful for scripting and automation, allowing you to extract version information for further processing or compatibility checks.

3. **`docker pull <image name>`**

   - **Explanation:** Pulls a Docker image from a registry (e.g., Docker Hub) to your local machine.
   - **Purpose:** Preparing your local environment by obtaining the necessary Docker images before running containers.

4. **`docker pull postgres`**

   - **Explanation:** Specifically pulls the PostgreSQL Docker image from Docker Hub.
   - **Purpose:** Fetching the PostgreSQL image for creating PostgreSQL database containers.

5. **`docker-compose`**

   - **Explanation:** A tool for defining and managing multi-container Docker applications using a YAML file.
   - **Purpose:** Simplifying the deployment and configuration of complex applications with multiple services, networks, and volumes.

6. **`docker image ls`**

   - **Explanation:** Lists all Docker images stored locally on your machine.
   - **Purpose:** Providing an overview of available images and their versions for reference or management.

7. **`docker image prune`**

   - **Explanation:** Removes unused Docker images to free up disk space.
   - **Purpose:** Managing storage by cleaning up images that are no longer in use.

8. **`docker ps`**

   - **Explanation:** Lists all currently running containers.
   - **Purpose:** Monitoring running containers and obtaining information such as container IDs, names, and resource usage.

9. **`docker run`**

   - **Explanation:** Creates and starts a Docker container based on a specified image.
   - **Purpose:** Instantiating and running applications or services within isolated containers.

10. **`docker stop <container id>`**

    - **Explanation:** Halts a running container.
    - **Purpose:** Gracefully stopping a container's execution.

11. **`docker run -e POSTGRES_PASSWORD=6862 ...`**

    - **Explanation:** Runs a container while setting an environment variable for configuring the PostgreSQL password.
    - **Purpose:** Providing initial configuration to containers, such as setting passwords dynamically.

12. **`docker run -d -p 5432:5432 --name postgres-old postgres:13.8`**

    - **Explanation:** Runs a container based on a specific version of the PostgreSQL image.
    - **Purpose:** Running containers with a specified image version for compatibility or testing.

13. **`docker container ls -a`**

    - **Explanation:** Lists all containers, including those that are stopped.
    - **Purpose:** Providing a comprehensive view of both running and stopped containers on the system.

14. **`docker container prune`**

    - **Explanation:** Removes all stopped containers.
    - **Purpose:** Cleanup, freeing up system resources by removing containers that are no longer needed.

15. **`docker volume ls`**

    - **Explanation:** Lists all volumes on the local machine.
    - **Purpose:** Managing persistent data by providing a way to store data independently of container lifecycles.

16. **`docker pull mongo`**

    - **Explanation:** Pulls the MongoDB Docker image from Docker Hub.
    - **Purpose:** Preparing to run MongoDB containers by obtaining the required image.

17. **`docker run -d -p 27017:27017 --name mongodb mongo`**

    - **Explanation:** Runs a MongoDB container in detached mode with port mapping.
    - **Purpose:** Launching a MongoDB container with port exposure for external access.

18. **`docker logs <container id>`**

    - **Explanation:** Displays the logs of a specific container.
    - **Purpose:** Troubleshooting and monitoring container output, useful for debugging.

19. **`docker logs -f <container id>`**

    - **Explanation:** Similar to the previous command but follows logs in real-time.
    - **Purpose:** Real-time monitoring of container logs for immediate feedback on container activities.

20. **`docker network ls`**

    - **Explanation:** Lists all Docker networks.
    - **Purpose:** Understanding and managing network configurations for container communication.

21. **`docker run -d -p 8081:8081 -e ME_CONFIG_MONGODB_ADMINUSERNAME=shivam ...`**
    - **Explanation:** Runs a container with specified environment variables for configuring a Mongo Express container.
    - **Purpose:** Setting up a Mongo Express container with username, password, and network configuration.

### Docker Compose Commands:

22. **`docker-compose --version`**

    - **Explanation:** Checks the version of Docker Compose installed on your system.
    - **Purpose:** Verifying the installed Docker Compose version for compatibility and feature availability.

23. **`docker-compose -f docker-compose.yaml up -d`**

    - **Explanation:** Runs a Docker Compose file, starting services defined in the specified YAML file in detached mode.
    - **Purpose:** Deploying multi-container applications with a single command and in a background (detached) mode.

24. **`docker-compose -f docker-compose.yaml down`**
    - **Explanation:** Stops and removes containers, networks, and volumes defined in the Docker Compose file.
    - **Purpose:** Gracefully shutting down and cleaning up resources associated with a multi-container application defined in a Compose file.
