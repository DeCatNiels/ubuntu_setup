# Start with the official Ubuntu base image
FROM ubuntu:latest

# Install sudo for testing container to mimic actual system
RUN apt-get update && apt-get install -y sudo openssh-client git curl

# Add the 'developer' user and set permisions
RUN useradd -m -s /bin/bash developer
RUN echo "developer ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/developer

# set default user
USER developer

# Set the working directory for the user
WORKDIR /home/developer

# Default command to run when the container starts
CMD ["/bin/bash"]