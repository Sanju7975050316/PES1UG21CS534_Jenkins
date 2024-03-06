#FROM jenkins/jenkins:lts
#FROM ubuntu:20.04
# if we want to install via apt
#USER root
#RUN apt-get update && apt-get install -y make && apt-get install -y g++ --fix-missing
# drop back to the regular jenkins user - good practice
#USER jenkins




# Use the official Jenkins LTS image based on Alpine
FROM jenkins/jenkins:lts-alpine

# Switch to root user for installation
USER root

# Update package repository and install required packages
RUN apk update && \
    apk add --no-cache make g++

# Switch back to the regular jenkins user (good practice)
USER jenkins
