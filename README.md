## Docker Installation on CentOS 7

1. **Update Package Repository:**
    ```bash
    sudo yum update
    ```

2. **Install Docker Dependencies:**
    ```bash
    sudo yum install -y yum-utils 
    ```

3. **Add Docker Repository:**
    ```bash    
    sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo --nogpgcheck

    ```

4. **Install Docker:**
    ```bash
    sudo yum install docker-ce 
    ```

5. **Start Docker Service:**
    ```bash
    sudo systemctl start docker
    ```

6. **Enable Docker on Boot:**
    ```bash
    sudo systemctl enable docker
    ```

7. **Verify Docker Installation:**
    ```bash
    sudo docker --version
    ```

For more details and updates, refer to the [official Docker documentation](https://docs.docker.com/install/linux/docker-ce/centos/).
