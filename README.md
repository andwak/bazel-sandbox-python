# Fix for DNS Name Resolve Issues
Open file `sudo nano /etc/resolv.conf`
Add nameserver 8.8.8.8 to use DNS server

# Install Docker
execute `sudo sh get-docker.sh`

# Reinstall WSL
Execute `wsl --list` to get instance name
Execute `wsl --unregister <instance_name>` to uninstall
Execute `wsl --install ubuntu` to install

# Build Docker Container
Execute `sudo docker build -t chart-drawer .` to build container

# Run the Docker Container
Execute `sudo docker run -i -t --rm -v ./src:/src chart-drawer` to run the container and mount the directory
