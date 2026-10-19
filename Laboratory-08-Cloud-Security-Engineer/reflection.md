# Mission Reflection

Completing Mission 8 helped me understand the importance of securing a cloud server instead of focusing only on making an application work.

A host-based firewall protects a server by controlling network traffic directly on the machine. Even if the physical network perimeter is breached, the firewall can still block incoming connections that are not allowed by its rules. This provides another layer of security for the server and its applications.

Managing open network ports is important because every exposed port can provide a possible entry point for attackers. By allowing only the services that are needed, administrators can reduce the server's attack surface and limit opportunities for unauthorized access.

In a real enterprise environment, leaving a database port such as MySQL's port 3306 open to the public internet is dangerous because attackers may attempt to exploit vulnerabilities, guess credentials, or access sensitive information. Database access should be restricted to authorized application servers and administrators instead of being publicly accessible.

This mission changed my perspective because I learned that a server can be exposed to risks when its network security is not configured properly. A working web application does not automatically mean that the server is secure. Configuring UFW, allowing SSH before enabling the firewall, and permitting TCP port 8080 showed me why security rules must be planned and verified carefully.

With eight completed missions, my GitHub portfolio now demonstrates a broader understanding of cloud computing, from deploying applications and managing infrastructure to monitoring and securing servers. It also provides organized documentation of my practical activities and the skills I have developed throughout the course. I can continue improving this portfolio by checking my work, documenting actual results, and applying security best practices in future projects.
