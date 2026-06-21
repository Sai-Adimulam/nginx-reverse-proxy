# nginx-reverse-proxy

1. User sends request

2. Nginx receives request on Port 80

3. Nginx forwards request to Flask App Port 5000

4. Flask processes request

5. Flask sends response to Nginx

6. Nginx returns response to User

Benefits of Nginx Reverse Proxy

✅ Hide application ports

✅ Load balancing

✅ SSL/HTTPS termination

✅ Better security

✅ Route traffic to multiple applications

Architecture:

without Nginx

User Browser
      |
      v
Flask Application
      |
      v
Port 5000 Exposed

Access: http://localhost:5000

With Nginx

User Browser
      |
      v
Nginx (Port 80)
      |
      v
Flask Application (Port 5000)

Access: http://localhost

