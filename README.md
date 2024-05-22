OpenStack Heat Templates
Brian Abshier 2024

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
