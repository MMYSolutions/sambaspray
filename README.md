# SambaSpray

> Deploy a Production Ready Samba4 Active Directory Domain Controller

[🇧🇷 Leia em Português](./README.pt-BR.md)

---

If you need to provision Samba4 Domain Controllers easily, following best practices and fully automated, **SambaSpray** is for you.
Inspired by [Kubespray](https://kubespray.io), this open source project leverages **Ansible** to simplify Samba4 deployments and streamline Active Directory management.

📣 **Community**
Questions? Suggestions? Join us on Telegram: [Samba4BR](https://t.me/samba4br).
You’ll find support, discussions, and contribute with PRs, Issues and feature ideas.

## ✅ Features

* Automated provisioning of **Samba4 Active Directory Domain Controllers**
* Integrated **DNS** configuration (Internal DNS)
* Supports multiple Linux distributions
* Modular and customizable architecture
* Production-ready deployment patterns\\

## ⚙️ Compatibility

SambaSpray can be deployed on:

* Bare Metal (physical servers)
* Virtual Machines (KVM, VMware, VirtualBox, Proxmox)
* Cloud Providers (AWS, Azure, GCP, etc.)

Supported Linux distributions:

* Oracle Linux 8

## 📦 Resources & Features

* High Availability

* Sysvol replication with GlusterFS

* Multiple Domain Controllers

* Multiple FileServers

* DNS SAMBA\_INTERNAL&#x20;

* Reverse DNS automatic creation

* Recycle Bin for deleted objects

* NTP Server configuration

* Backup of Domain Controllers with custom scripts

## 🛠️ Requirements

* Ansible >= 2.14
* Python >= 3.8
* sshpass (for automated SSH connections)
* Servers with root or sudo access
* Internet access (for package installation)

### Required Packages

#### APT-based systems (Debian, Ubuntu):

```bash
apt-get update
apt-get install python3-pip git sshpass -y
pip3 install pip --upgrade
pip3 install ansible
```

#### YUM-based systems (CentOS, Oracle, Rocky, Alma):

```bash
yum install python3-pip git sshpass -y
pip3 install pip --upgrade
pip3 install ansible
```

## 🚀 Quick Start

Clone the repository:

```bash
git clone https://github.com/ybucci/samba4spray.git
cd samba4spray
```

Configure your inventory:

```bash
nano inventory/cliente1/hosts.ini
```

Run the playbook from your Ansible machine:

```bash
ansible-playbook --become -i inventory/cliente1/hosts.ini install.yml
```

## 🌱 Roadmap

* Upgrade playbook

* Bind9 (named) support

* SSL/TLS

* Encryption in Transit / Encryption at rest

* Complete documentation (EN & PT-BR)

## 🤝 Contributing

We welcome your contributions to SambaSpray!
Whether it's opening Issues, submitting Pull Requests, or suggesting improvements, your collaboration helps us grow.

Let's build the leading open source automation solution for Samba4 together!

**Community hub:** [Samba4BR on Telegram](https://t.me/samba4br)

## 📝 License

MIT License - Use it, share it, contribute back.
