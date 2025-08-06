## 📘 Ansible Playbooks Repository

### Overview

This repository contains Ansible playbooks designed to automate common infrastructure and application deployment tasks. Built for DevOps and cloud-first environments, these playbooks make it easy to provision servers, install software, manage services, and deploy applications.

---

### 🛠️ Features

* **Structured playbooks** for web servers, applications, and environment configuration
* **Reusable roles** to keep tasks DRY and modular
* Examples for common operations like installing packages, copying files, starting services
* Focus on **cloud deployments** (AWS EC2, t2.micro, Ubuntu, Amazon Linux)

---

   

### ⚙️ Sample Inventory: `inventory/hosts.ini`

```ini
[web]
192.0.2.10 ansible_user=ec2-user ansible_ssh_private_key_file=~/.ssh/mykey.pem
```

---

### 🧩 Configuration: `ansible.cfg`

```ini
[defaults]
inventory = inventory/hosts.ini
host_key_checking = False
remote_user = ec2-user
```

---

### ✅ Usage Flow

1. Clone the repo:

   ```bash
   git clone https://github.com/Avnish-web/Ansible-Playbooks.git
   cd Ansible-Playbooks
   ```
2. Review and adjust the inventory file.
3. Ensure your SSH key is authorized on remote hosts.
4. Run one of the playbook

---

### 📚 Learn More

* Ansible playbooks are YAML-based workflows that automate tasks across many hosts ([github.com][1], [docs.ansible.com][2], [github.com][3], [docs.ansible.com][4])
* Roles help you modularize and reuse task logic across playbooks ([docs.ansible.com][5])

---

### 🧡 Contributions Welcome

Feel free to contribute by:

* Adding more playbooks or roles
* Improving existing ones
* Enhancing documentation or examples

---

### 📄 License

Open-source and licensed under the MIT License.
