# 🚀 Liferay Workspace Setup Guide
Follow these steps in the correct order to successfully set up and run your Liferay workspace using Docker and Blade CLI.

### 🧰 Prerequisites
Make sure you have the following installed:

Blade CLI

Docker

Git

### 🔧 Setup Instructions
1️⃣ Clone the Repository

git clone <your-repo-url>
cd <your-project-directory>

### 2️⃣ Initialize Blade Server
Run the following inside the project directory:

blade server init

### 3️⃣ Add the Database Driver
Add the appropriate database driver .jar file to:

./bundles/osgi/modules

📌 Example: For MySQL, add mysql-connector-java-<version>.jar.

### 4️⃣ Start the Docker Containers
Use Docker Compose to spin up the required containers:

docker-compose up -d

This may take a few minutes the first time it runs.

### 5️⃣ Run the Liferay Server
Start the Liferay server with Blade CLI:

blade server run

Wait for the server to fully start.

### 🌐 Access Liferay
Once the project is running, open your browser and go to:

http://localhost:8080

### 🔐 First-Time Login

Email/Username: test@liferay.com

Password: test

👉 You'll be prompted to set a custom password after logging in for the first time.
Use the credentials provided in the docker-compose.yaml file or come up with an own password. Write it down somewhere because you will need it everytime you access the application. 
