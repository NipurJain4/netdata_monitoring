In this task, we'll use Netdata, an open-source monitoring tool, to keep an eye on our system and application performance. We'll run it inside Docker and explore its dashboard to see live metrics like CPU, memory, disk usage, and even Docker container stats.
🎯 Objective
Set up Netdata, access its dashboard, and explore live system and app performance metrics.
🛠 Tools Needed
• Netdata (Free and open-source monitoring tool)
• Docker installed on your system
🚀 Steps to Install & Run Netdata in Docker
1. Make sure Docker is installed and running on your system.
2. Open your terminal and pull + run the Netdata container:
   docker run -d --name=netdata -p 19999:19999 netdata/netdata
3. Once the container is up, open your browser and go to:
   http://localhost:19999
4. Explore the dashboard — check CPU load, memory usage, disk activity, and container metrics.
5. Check out the alerts and different chart panels to get insights into system health.
6. To view Netdata logs, run:
   docker exec -it netdata cat /var/log/netdata/error.log
  ![netstat Dashboard]()
