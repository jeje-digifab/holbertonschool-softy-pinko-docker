### Task 2: Front-end

**Objective**: Create a front-end to display content from the back-end API.

**Description**:
- This task involves setting up a front-end to interact with the back-end API created in the previous task.
- The front-end is served using Nginx, a popular web server.
- The front-end content is cloned from a provided repository and configured to be served by Nginx.
- The front-end makes API calls to the back-end to fetch dynamic data.

**Steps**:
1. **Reorganize Project Structure**:
   - Create separate directories for the back-end and front-end.
   - Move the back-end files into the `back-end` directory.
   - Create a new `front-end` directory and clone the front-end repository into it.

2. **Create Dockerfile for Front-end**:
   - Use the latest Nginx image as the base.
   - Copy the front-end files to the appropriate directory in the Docker image.
   - Create an Nginx configuration file to serve the front-end content.

3. **Configure Nginx**:
   - Create an Nginx configuration file (`softy-pinko-front-end.conf`) to set up the server.
   - Ensure the configuration includes settings for the server name, port, and location of the front-end files.

4. **Build and Run Docker Images**:
   - Build the Docker images for both the back-end and front-end.
   - Run the Docker containers, ensuring the front-end can communicate with the back-end API.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task2`

This task focuses on setting up a front-end that interacts with a back-end API, demonstrating how to serve static content using Nginx and fetch dynamic data from a Flask-based back-end.
