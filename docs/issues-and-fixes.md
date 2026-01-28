# Issues Faced and Fixes During Java App Deployment

This file explains the problems I faced while deploying my Java application on AWS EC2 and how I fixed them.

---

Issue 1: 502 Bad Gateway

Problem:
The website showed a 502 Bad Gateway error.

Reason:
The Java application was not running on port 8080.

Fix:
I started the Java application and verified it using:
curl http://localhost:8080

Result:
The error was resolved.

---

Issue 2: SSL Failed for www Domain

Problem:
SSL certificate generation failed.

Reason:
The www subdomain DNS record was missing.

Fix:
I edited the DNS record and pointed www to the EC2 public IP.

Result:
SSL was generated successfully.

---

Issue 3: HTTPS Not Opening

Problem:
The website did not open on HTTPS.

Reason:
Port 443 was blocked in the EC2 security group.

Fix:
I allowed port 443 in the inbound rules.

Result:
HTTPS started working.

---

Issue 4: Nginx Configuration Error

Problem:
Nginx failed to start.

Reason:
proxy_pass was placed in the wrong location.

Fix:
I moved proxy_pass into the correct server and location block.

Result:
Nginx started successfully.

---

Final Result:
The Java application is running with domain mapping and HTTPS enabled.
