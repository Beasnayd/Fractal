# Fractal

### 1. **System Requirements**
   - **Operating System:** Ubuntu 20.04 LTS (recommended).
   - **Hardware:** A server with at least 8 CPU cores, 16GB RAM, 500GB SSD, and a stable internet connection with at least 1Gbps bandwidth.

### 2. **Server Preparation**
   - **Update and Upgrade your system:**
     ```bash
     sudo apt update && sudo apt upgrade -y
     ```
   - **Install essential packages:**
     ```bash
     sudo apt install curl git build-essential -y
     ```

### 3. **Installing Fractal Node Software**
   Fractal provides a **Validator Toolbox** that simplifies the installation and management of your node.

   - **Download the Validator Toolbox:**
     ```bash
     git clone https://github.com/fractal-bitcoin/fractal
     cd fractal
     ```

   - **Run the installation script:**
     ```bash
     ./install.sh
     ```
     This script will install all necessary dependencies and configure your node.

### 4. **Node Configuration**
   After installation, configure your node:
   - **Edit the configuration file:** You will find the configuration file within the `fractal` directory.
     ```bash
     nano config.toml
     ```
     Adjust the parameters according to your setup, including setting your node name, configuring ports, and connecting to peers.

### 5. **Starting Your Node**
   Once everything is configured:
   - **Initialize the node:**
     ```bash
     ./fractal-node init
     ```
   - **Start the node:**
     ```bash
     ./fractal-node start
     ```
   Monitor the logs to ensure the node is syncing correctly.

### 6. **Validator Setup**
   To become a validator:
   - **Stake FRA tokens** to your validator address.
   - **Register your validator** on the network through the provided CLI commands or via the Fractal staking portal.

### 7. **Monitoring and Maintenance**
   - **Regularly update your node** using the toolbox's update functionality to stay in sync with network upgrades.
   - **Monitor your node's performance** using the built-in monitoring tools within the Validator Toolbox.

For a detailed guide and additional options, you can refer to the official [Fractal Validator Documentation](https://docs.fra.tech/validator-materials/node-setup-guides/validator-toolbox-setup).
