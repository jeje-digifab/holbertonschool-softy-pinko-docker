### README Summary

This project involves creating and managing Docker images and containers for a simple web application. The tasks progress from creating a basic Docker image to setting up a full-stack application with a front-end, back-end, and proxy server, all managed using Docker Compose. Below is a summary of each task:

#### Task 0: Create Your First Docker Image
- **Objective**: Create a Docker image that echoes "Hello, World!" when run.
- **Steps**:
  - Use a Dockerfile based on the latest Ubuntu image.
  - Update APT and upgrade installed software.
  - Build and run the Docker image to display "Hello, World!" in the terminal.

#### Task 1: Back-end
- **Objective**: Set up a back-end server using Flask.
- **Steps**:
  - Copy the Task 0 directory to Task 1.
  - Modify the Dockerfile to install Python3, pip3, and Flask.
  - Create a Python script (`api.py`) to run a Flask server with an endpoint that returns "Hello, World!".
  - Build and run the Docker image, ensuring the Flask server is accessible on port 5252.

#### Task 2: Front-end
- **Objective**: Create a front-end to display content from the back-end API.
- **Steps**:
  - Copy the Task 1 directory to Task 2.
  - Reorganize the project structure to separate back-end and front-end.
  - Create a Dockerfile for the front-end using Nginx.
  - Clone a front-end repository and configure Nginx to serve the front-end content.
  - Build and run the front-end Docker image, ensuring it is accessible on port 9000.

#### Task 3: Connecting the Front-end and Back-end
- **Objective**: Connect the front-end to the back-end to display dynamic data.
- **Steps**:
  - Copy the Task 2 directory to Task 3.
  - Modify the front-end HTML to include a dynamic content section.
  - Add JavaScript to fetch data from the back-end API.
  - Modify the back-end to use Flask-CORS for cross-origin requests.
  - Build and run both front-end and back-end Docker images, ensuring they communicate correctly.

#### Task 4: Making it Simpler with Docker Compose
- **Objective**: Use Docker Compose to manage multiple containers.
- **Steps**:
  - Copy the Task 3 directory to Task 4.
  - Create a `docker-compose.yml` file to define services for the back-end, front-end, and proxy.
  - Build and run the services using Docker Compose.

#### Task 5: Proxy Server
- **Objective**: Set up a proxy server to route requests to the front-end and back-end.
- **Steps**:
  - Copy the Task 4 directory to Task 5.
  - Create a proxy directory with a Dockerfile and Nginx configuration.
  - Modify the front-end JavaScript to make API calls through the proxy.
  - Update the `docker-compose.yml` file to include the proxy service.
  - Build and run the services, ensuring all requests are routed through the proxy.

#### Task 6: Scale Horizontally
- **Objective**: Scale the back-end by adding multiple API servers and load-balance requests.
- **Steps**:
  - Copy the Task 5 directory to Task 6.
  - Modify the `docker-compose.yml` file to launch multiple back-end containers.
  - Use Nginx as a load balancer to distribute requests among the back-end servers.
  - Build and run the services, ensuring requests are load-balanced across multiple back-end servers.

### Repository Information
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directories**:
  - Task 0: `task0`
  - Task 1: `task1`
  - Task 2: `task2`
  - Task 3: `task3`
  - Task 4: `task4`
  - Task 5: `task5`
  - Task 6: `task6`

This summary provides an overview of the tasks and the progression from a simple Docker image to a fully functional, scalable web application managed with Docker Compose.