# Base Image 
FROM ubuntu:16.04 

# Maintainer of this Image 
MAINTAINER Amit Vashist <amitvashist7@outlook.com>

# Update the APT Repos 
RUN apt-get update 

# Install Apache Package 
RUN apt-get install apache2 -y 

# Bring up the Apache Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
