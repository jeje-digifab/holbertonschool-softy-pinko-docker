### Task 1: Back-end

**Objective**: Set up a back-end server using Flask.

**Description**:
- This task involves creating a back-end server using Flask, a lightweight WSGI web application framework in Python.
- The back-end server is set up to handle API requests and return a simple "Hello, World!" message.
- The Dockerfile is modified to install Python3, pip3, and Flask, and to copy the necessary Python script into the Docker image.
- The Flask server is configured to run on port 5252 and is accessible from outside the Docker container.

**Steps**:
1. **Copy Task 0 Directory**:
   - Start by making a copy of the Task 0 directory and naming it Task 1.

2. **Modify Dockerfile**:
   - Update the Dockerfile to install Python3, pip3, and Flask.
   - Ensure the Dockerfile copies the Python script (`api.py`) into the Docker image.

3. **Create Python Script**:
   - Create a Python script (`api.py`) that sets up a Flask server with an endpoint returning "Hello, World!".
   - The Flask server is configured to run on `0.0.0.0` and port 5252, making it accessible from outside the Docker container.

4. **Build and Run Docker Image**:
   - Build the Docker image using the modified Dockerfile.
   - Run the Docker container, ensuring the Flask server is accessible on port 5252.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task1`

This task focuses on setting up a back-end server using Flask, demonstrating how to create a simple API endpoint and serve it using Docker.
