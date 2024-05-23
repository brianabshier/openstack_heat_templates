## OpenStack Heat Templates

<sup>Brian Abshier 2024</sup>

---

### quick_create_heat_template.yaml

- **Description:** Basic Heat template that creates a VM with an existing key for authentication, and all the prerequisites on the networking side to make it publicly accessible.

**Resources Created:**

- **Network**: A private network for the VM.
- **Subnet**: A subnet within the private network.
- **Router**: A router to connect the private network to the public network.
- **Router Interface**: An interface to connect the router to the subnet.
- **Port**: A network port for the VM.
- **Security Group**: A security group with rules to allow SSH and ICMP.
- **Floating IP**: A floating IP to make the VM publicly accessible.
- **VM Instance**: The VM instance configured with the specified parameters.
---

### quick_LAMP_heat_template.yaml

- **Description:** Provisions a virtual machine with a specified flavor, image, and SSH key, sets up a private network and subnet, configures routing to an external network, and installs a LAMP stack (Linux, Apache, MySQL, PHP) on the instance. It includes security group rules to allow SSH, HTTP, and HTTPS access and assigns a floating IP to the instance for public accessibility.

**Resources Created:**

- **Network**: A private network for the VM.
- **Subnet**: A subnet within the private network.
- **Router**: A router to connect the private network to the public network.
- **Router Interface**: An interface to connect the router to the subnet.
- **Port**: A network port for the VM.
- **Security Group**: A security group with rules to allow SSH and ICMP.
- **Floating IP**: A floating IP to make the VM publicly accessible.
- **VM Instance**: The VM instance configured with the specified parameters.

**Software Installed:**

- **Apache**: A web service.
- **MySQL**: A relational database service.
- **PHP**: An open source scripting language

---

### openstack_wordpress_single_stack.yaml

- **Description:** Deploys a WordPress server on OpenStack with a local mysql database. This will create the necessary network infrastructure, security groups, and a VM instance. You will need to log into your server's wp-admin URL to complete the installation

**Resources Created:**

- **Network**: A private network for the VM.
- **Subnet**: A subnet within the private network.
- **Router**: A router to connect the private network to the public network.
- **Router Interface**: An interface to connect the router to the subnet.
- **Port**: A network port for the VM.
- **Security Group**: A security group with rules to allow SSH and ICMP.
- **Floating IP**: A floating IP to make the VM publicly accessible.
- **VM Instance**: The VM instance configured with the specified parameters.

**Software Installed:**

- **Apache**: A web service.
- **MySQL**: A relational database service.
- **PHP**: An open source scripting language
- **WordPress**: A web content management system.
