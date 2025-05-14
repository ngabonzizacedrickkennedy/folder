Summary of Complete Project Setup
Here's a comprehensive summary of what we've accomplished for both parts of your project:
Apache Setup (First Virtual Interface)

Virtual Interface Configuration

Set up the first virtual interface (eth0.100) with IP 192.168.43.224
Verified the interface was properly configured and active


Apache2 Installation and Configuration

Installed and configured Apache2 web server
Created a virtual host configuration for the domain 25503.auca.ac.rw
Configured Apache to listen on the virtual interface IP
Set up the document root at /var/www/auca-education


Web Content Creation

Created a static HTML page for AUCA Education
Added your student information (ID: 25503, Name: Ngabonziza Cedrick Kennedy)
Set proper permissions for the web files


Domain Configuration

Added entry in the hosts file for 25503.auca.ac.rw
Verified the domain resolution was working correctly


Testing

Confirmed that Apache was serving the static AUCA Education page
Accessed the site successfully via the configured domain name



Nginx Portfolio Setup (Second Virtual Interface)

Virtual Interface Configuration

Set up the second virtual interface (eth0.200) with IP 192.168.43.225
Verified the interface was properly configured and active


Database Installation and Configuration

Installed and configured MariaDB for the portfolio database
Created a database called portfolio_db
Set up a database user with appropriate permissions
Created necessary tables: user_info, skills, and experience
Populated the tables with initial data


Web Server Installation and Configuration

Installed Nginx and PHP-FPM (php8.4-fpm)
Configured Nginx to listen on port 8080 on the second virtual interface
Set up PHP-FPM to process PHP files
Created a server configuration for portfolio.auca.ac.rw


Dynamic Portfolio Website

Created the directory structure at /var/www/portfolio
Implemented the PHP files (index.php and process.php)
Set up the file upload functionality for profile pictures
Configured proper file permissions


Portfolio Features

Implemented light/dark theme switching functionality
Created CRUD operations for profile, skills, and experience
Set up dynamic data retrieval from the database
Configured the user interface with interactive elements


Performance Optimization

Configured PHP-FPM with optimized settings
Fine-tuned Nginx for better performance
Adjusted MariaDB for improved database operations


Testing

Verified Nginx was listening on the correct port and IP
Successfully accessed the portfolio through a web browser
Confirmed all dynamic functionality was working



Current Status

AUCA Education Site: Accessible via HTTP at http://25503.auca.ac.rw
Portfolio Site: Accessible via HTTP at http://portfolio.auca.ac.rw:8080
Both sites are operational and meet the basic requirements of the project

Remaining Tasks

Security Implementation

Set up HTTPS with self-signed certificates for both sites
Install and configure ModSecurity for Apache and Nginx
Implement firewall rules with UFW
Configure two-factor authentication for SSH


Docker Deployment (Part 2)

Containerize the portfolio application
Set up Traefik as a load balancer
Configure high availability across multiple nodes



The project has successfully implemented the core requirements of hosting two different web services on
separate virtual interfaces, with the first serving a static site and the second providing a dynamic portfolio 
system with database integration.
