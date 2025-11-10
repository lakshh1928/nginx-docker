========================================
🎮 Simon Game - Dockerized Nginx Setup
========================================

📌 Project Overview
-------------------
This project is a simple web-based version of the classic **Simon Game**, 
developed using HTML, CSS, and JavaScript. 
The application is containerized using **Docker** and served using **Nginx** 
with **reverse proxy** and **load balancing** configuration.

This setup demonstrates how to:
- Host a static web app using Nginx inside Docker
- Configure a reverse proxy
- Load balance between multiple app containers
- Expose the app to the internet using tools like ngrok

🤝 Collaboration
----------------
This project is a collaboration between **Archit** and **Laksh**.

📂 Project Structure
--------------------
/home/l4ksh/project/Simon-game/
│
├── index.html
├── style.css
├── index.js
├── nginx.conf              # Nginx reverse proxy config
├── Dockerfile              # Build static app image
├── docker-compose.yml      # Multi-container setup
└── README.txt

⚙️ How to Run
-------------
1. Clone the repository:
   git clone <repo-url>

2. Navigate into the project folder:
   cd Simon-game

3. Build and run the containers:
   docker compose up --build -d

4. Access the game:
   http://localhost:8080

   (If using ngrok)
   ngrok http 8080

   Copy the public ngrok URL to share the game.

🌐 Features
-----------
- Fully containerized setup using Docker Compose
- Nginx reverse proxy configuration
- Load balancing between two app instances
- Custom headers to identify backend containers
- Easily deployable to any cloud or VPS

📜 Logs and Monitoring
----------------------
To view Nginx access logs:
   docker logs -f proxy

To view app logs:
   docker logs app1
   docker logs app2

🧠 Learning Highlights
----------------------
This project helped in understanding:
- Docker image creation and container orchestration
- Nginx as a web server and load balancer
- Basic DevOps deployment concepts
- Using ngrok for public sharing

🚀 Future Improvements
----------------------
- Add HTTPS (SSL) using Let's Encrypt
- Deploy on a cloud server (AWS/DigitalOcean)
- Add CI/CD pipeline for automated deployment

----------------------------------------
💡 Created by Archit & Laksh (DevOps Practice Project)
----------------------------------------

