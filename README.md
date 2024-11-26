# **Cintel-05-Cintel: Module 5 - Live Data with PyShiny**

## **Overview**
This project demonstrates how to use Python's `deque` and PyShiny's reactive values to integrate live data updates into a PyShiny application. The dashboard visualizes real-time Antarctic temperature readings with interactive charts and dynamic updates.

---

## **Features**
- Live data updates with customizable intervals.
- Interactive charts displaying temperature trends.
- Implementation of `deque` for efficient data handling.
- Dynamic, responsive PyShiny UI.

---

## **Setup Instructions**

### **1. Create and Activate the Virtual Environment**

# Create virtual environment
py -m venv .venv

# Activate virtual environment
.venv\Scripts\Activate

### 2. Install Dependencies
Install all required packages using requirements.txt and ensure they are up-to-date:



py -m pip install --upgrade -r requirements.txt

### 3. Update Dependencies
After making any changes to dependencies, update the requirements.txt file:


py -m pip freeze > requirements.txt
Additional Dependencies
Install WebSocket-related packages:


# Install websocket-client
py -m pip install websocket-client

# Install a specific version of websockets (10.4)
py -m pip install websockets==10.4
Building the Client-Side App
To create and serve the client-side build of the PyShiny application:

Remove Static Assets (if necessary):


shiny static-assets remove
Export for Shinylive:


shinylive export dashboard docs
Start a Local Server:

py -m http.server --directory docs --bind localhost 8008
Access the Application: Open your web browser (e.g., Chrome) and navigate to:


http://localhost:8008
Updating the GitHub Repository
After making changes locally, follow these steps to push updates to your GitHub repository:

# Stage all changes
git add .

# Commit changes with a descriptive message
git commit -m "Update GitHub Repository with local build and add to Pages"

# Push changes to the remote repository
git push -u origin main
Live Demo
You can view the live version of this application hosted on GitHub Pages:
https://claytonseabaughgh.github.io/cintel-05-cintel/

Resources
PyShiny Documentation
Shinylive Documentation
GitHub Repository
vbnet








