### Task 5: Proxy Server

**Objective**: Set up a proxy server to route requests to the front-end and back-end.

**Description**:
- This task involves setting up a proxy server using Nginx to route requests between the front-end and back-end.
- The proxy server acts as an intermediary, forwarding requests to the appropriate service based on the URL path.
- This setup simplifies the client-side configuration by providing a single entry point for all requests.

**Steps**:
1. **Copy Task 4 Directory**:
   - Start by making a copy of the Task 4 directory and naming it Task 5.

2. **Create Proxy Directory**:
   - Inside the Task 5 directory, create a new folder named `proxy`.

3. **Create Dockerfile for Proxy**:
   - In the `proxy` directory, create a Dockerfile that uses the latest version of Nginx.
   - Create a configuration file named `proxy.conf` to define the proxy settings.
   - Ensure the Dockerfile copies the `proxy.conf` file to `/etc/nginx/conf.d/default.conf` in the Docker image.

4. **Configure Proxy**:
   - In the `proxy.conf` file, set up the server to listen on port 80.
   - Define location blocks to route requests to the front-end and back-end services.
   - Use the service names defined in the `docker-compose.yml` file for routing.

5. **Update `docker-compose.yml`**:
   - Add a new service for the proxy in the `docker-compose.yml` file.
   - Ensure the proxy service maps the container's port 80 to the host machine's port 80.
   - Remove the port mappings for the front-end and back-end services to ensure all requests go through the proxy.

6. **Modify Front-end JavaScript**:
   - Update the JavaScript in the `index.html` file to make API requests through the proxy server.
   - Change the API endpoint URL to `/api/hello`.

7. **Build and Run Services**:
   - Use Docker Compose to build and run the services defined in the `docker-compose.yml` file.
   - Ensure the proxy server correctly routes requests to the front-end and back-end services.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task5`

This task demonstrates how to set up a proxy server using Nginx to route requests between the front-end and back-end services, simplifying the client-side configuration and providing a single entry point for all requests.
