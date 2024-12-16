### Task 4: Making it Simpler with Docker Compose

**Objective**: Use Docker Compose to manage multiple containers.

**Description**:
- This task involves using Docker Compose to simplify the management of multiple Docker containers.
- Docker Compose allows you to define and run multi-container Docker applications with a single configuration file.
- The `docker-compose.yml` file is created to define services for the back-end, front-end, and proxy.
- This setup ensures that all containers are started and managed together, making it easier to handle complex applications.

**Steps**:
1. **Copy Task 3 Directory**:
   - Start by making a copy of the Task 3 directory and naming it Task 4.

2. **Create `docker-compose.yml` File**:
   - Inside the Task 4 directory, create a `docker-compose.yml` file.
   - Define the services for the back-end, front-end, and proxy in the `docker-compose.yml` file.
   - Include necessary configurations such as build context, Dockerfile, image, ports, and dependencies.

3. **Build and Run Services**:
   - Use Docker Compose to build the services defined in the `docker-compose.yml` file.
   - Run the services using Docker Compose, ensuring all containers are started and managed together.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task4`

This task focuses on using Docker Compose to manage multiple containers, simplifying the process of running and managing complex Docker applications. It demonstrates how to define and run multi-container applications with a single configuration file.
