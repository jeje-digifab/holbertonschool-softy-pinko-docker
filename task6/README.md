### Task 6: Scale Horizontally

**Objective**: Scale the back-end by adding multiple API servers and load-balance requests.

**Description**:
- This task involves scaling the back-end by adding multiple API servers and using Nginx as a load balancer to distribute requests among them.
- The goal is to handle increased traffic by distributing the load across multiple back-end servers, ensuring better performance and reliability.
- Docker Compose is used to manage the multiple back-end containers and the load balancer.

**Steps**:
1. **Copy Task 5 Directory**:
   - Start by making a copy of the Task 5 directory and naming it Task 6.

2. **Modify `docker-compose.yml`**:
   - Update the `docker-compose.yml` file to launch multiple instances of the back-end service.
   - Use the `scale` option in Docker Compose to specify the number of back-end instances to run.

3. **Configure Nginx for Load Balancing**:
   - Ensure the Nginx configuration in the proxy service is set up to load balance requests across the multiple back-end instances.
   - Use the Round-Robin algorithm to distribute requests evenly among the back-end servers.

4. **Create Command File**:
   - Create a file named `2-api-servers.txt` in the Task 6 directory.
   - Include the exact Docker Compose command used to spin up the multiple back-end instances.

5. **Build and Run Services**:
   - Use Docker Compose to build and run the services defined in the `docker-compose.yml` file.
   - Ensure the load balancer correctly distributes requests among the multiple back-end instances.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task6`

This task demonstrates how to scale a back-end service horizontally by adding multiple API servers and using Nginx as a load balancer. This setup ensures better performance and reliability by distributing the load across multiple back-end instances
