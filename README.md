LAMP Stack Deployment on Kubernetes Using Ansible & KIND
✅ Project Overview
This project provisions a LAMP (Linux, Apache, MySQL, PHP) stack on a Kubernetes cluster using Ansible automation.
The Kubernetes cluster is created using KIND (Kubernetes in Docker), and all Docker images are built manually (no pre-built images from Docker Hub).

Tech Stack
Kubernetes (KIND) – Lightweight Kubernetes cluster
Ansible – Infrastructure automation & deployment
Docker – Custom-built images (Apache, MySQL, PHP)
Linux (Ubuntu Base) – Base OS for Docker images
Persistent Volumes (PV & PVC) – For MySQL data storage

Features
✔ Custom Docker images for Apache, MySQL, and PHP
✔ Automated deployment using Ansible Playbooks
✔ Persistent storage for MySQL using PV & PVC
✔ Single-node Kubernetes Cluster (KIND)
✔ Tested PHP → MySQL database connection

Folder Structure
lamp-ansible-k8s/
├── ansible/
│   ├── inventory.ini
│   ├── playbook.yml
├── dockerfiles/
│   ├── apache/
│   │   └── Dockerfile
│   ├── mysql/
│   │   └── Dockerfile
│   └── php/
│       ├── Dockerfile
│       └── test.php
├── k8s-manifests/
│   ├── persistent-volume.yml
│   ├── mysql-deployment.yml
│   ├── apache-deployment.yml
│   └── php-deployment.yml
└── README.md
