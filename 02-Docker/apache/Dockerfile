# Base Image
FROM ubuntu:latest

# Owner
MAINTAINER Amit Vashist  <av@gmail.com>

# Update  Apt Repo
RUN apt-get update

# Install Apache Pacakges 
RUN apt-get install apache2 -y

# Deploy Index File.
COPY amit.html /var/www/html/index.html

#Expose Service
EXPOSE 80

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND" ]
