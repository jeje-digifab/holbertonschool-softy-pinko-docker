### Task 3: Connecting the Front-end and Back-end

**Objective**: Connect the front-end to the back-end to display dynamic data.

**Description**:
- This task involves integrating the front-end with the back-end to enable dynamic data display.
- The front-end is modified to include a new HTML element for dynamic content.
- JavaScript is used to make API requests to the back-end and update the front-end with the fetched data.
- The back-end is updated to handle cross-origin requests using Flask-CORS.

**Steps**:
1. **Copy Task 2 Directory**:
   - Start by making a copy of the Task 2 directory and naming it Task 3.

2. **Modify Front-end HTML**:
   - Add a new `<h1>` tag with the ID `dynamic-content` before the existing content in the `index.html` file.
   - This tag will be used to display dynamic data fetched from the back-end API.

3. **Add JavaScript for API Request**:
   - Include a JavaScript script at the bottom of the `index.html` file to make an API request to the back-end.
   - The script fetches data from the back-end API endpoint and updates the `dynamic-content` element with the fetched data.

4. **Update Back-end for CORS**:
   - Modify the back-end Dockerfile to install Flask-CORS.
   - Update the `api.py` script to use Flask-CORS, allowing the back-end to handle cross-origin requests from the front-end.

5. **Build and Run Docker Images**:
   - Build the Docker images for both the front-end and back-end.
   - Run the Docker containers, ensuring the front-end can communicate with the back-end API and display dynamic data.

**Repository Information**:
- **GitHub Repository**: [holbertonschool-softy-pinko-docker](https://github.com/holbertonschool-softy-pinko-docker)
- **Directory**: `task3`

This task demonstrates how to connect a front-end to a back-end API, enabling dynamic data display on the front-end. It involves modifying both the front-end and back-end to ensure seamless communication and data retrieval.
