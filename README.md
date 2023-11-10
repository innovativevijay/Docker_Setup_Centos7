## Docker Installation on CentOS 7
Docker is a platform for developing, shipping, and running applications in containers. To install Docker on CentOS 7:
1. **Update Package Repository:**
- Description: Updates the package repository to ensure you have the latest package information.
   ```bash
    sudo yum update
    ```

3. **Install Docker Dependencies:**
- Description: Installs necessary dependencies for Docker to function properly.
   ```bash
    sudo yum install -y yum-utils 
    ```

5. **Add Docker Repository:**
- Description: Adds the Docker repository to your system's package manager configuration.
   ```bash    
    sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo --nogpgcheck

    ```

7. **Install Docker:**
- Description: Installs Docker packages, including the Docker engine, command-line client, and container runtime.

    ```bash
    sudo yum install docker-ce 
    ```

9. **Start Docker Service:**
- Description: Starts the Docker service to enable container management.
    ```bash
    sudo systemctl start docker
    ```

11. **Enable Docker on Boot:**
- Description: Configures Docker to start automatically on system boot.
     ```bash
    sudo systemctl enable docker
    ```

13. **Verify Docker Installation:**
- Description: Verifies the successful installation of Docker and displays the version.
     ```bash
    sudo docker --version
    ```

For more details and updates, refer to the [official Docker documentation](https://docs.docker.com/install/linux/docker-ce/centos/).
