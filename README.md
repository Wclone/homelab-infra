# Homelab Infrastructure: A DevOps Learning Journey 🌐

Welcome to the **Homelab Infrastructure** repository! This project aims to enhance your DevOps skills through hands-on experience with real infrastructure components. Here, you'll explore K3s, Docker, self-hosted stacks, and Infrastructure as Code (IaC). 

[![Releases](https://img.shields.io/badge/Releases-v1.0.0-blue)](https://github.com/Wclone/homelab-infra/releases)

## Table of Contents

1. [Introduction](#introduction)
2. [Technologies Used](#technologies-used)
3. [Getting Started](#getting-started)
4. [Project Structure](#project-structure)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

---

## Introduction

In today's fast-paced tech world, understanding DevOps practices is crucial. This repository provides a practical approach to learning by building a homelab. You'll work with tools and technologies that are widely used in the industry. Whether you're a beginner or looking to sharpen your skills, this project offers valuable insights.

## Technologies Used

This project incorporates a variety of technologies, including:

- **K3s**: A lightweight Kubernetes distribution.
- **Docker**: For containerization of applications.
- **MariaDB**: An open-source database management system.
- **Plex Media Server**: For media streaming.
- **Adminer**: A database management tool.
- **Tailscale**: For secure networking.
- **Vaultwarden**: A self-hosted password manager.
- **Automation Tools**: To streamline deployment and management.
- **CI/CD Pipelines**: For continuous integration and delivery.

## Getting Started

To get started with the project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Wclone/homelab-infra.git
   cd homelab-infra
   ```

2. **Download and Execute Releases**:
   Visit the [Releases section](https://github.com/Wclone/homelab-infra/releases) to download the latest release files. Execute them according to the instructions provided in the release notes.

3. **Set Up Your Environment**:
   Ensure you have the following prerequisites installed:
   - Docker
   - kubectl
   - Helm (for managing Kubernetes applications)

4. **Deploy the Stack**:
   Follow the provided scripts and documentation to deploy the entire stack. Each component will have its configuration files to customize the setup to your needs.

## Project Structure

The repository is organized as follows:

```
homelab-infra/
├── docker/
│   ├── docker-compose.yml
│   └── .env
├── k3s/
│   ├── k3s-install.sh
│   └── k3s-config.yaml
├── mariadb/
│   ├── init.sql
│   └── docker-compose.yml
├── plex/
│   ├── plex-docker-compose.yml
│   └── plex-config/
├── tailscale/
│   └── tailscale-config.yaml
└── vaultwarden/
    ├── vaultwarden-docker-compose.yml
    └── .env
```

### Description of Key Directories

- **docker/**: Contains Docker-related files, including `docker-compose.yml` for orchestrating multi-container applications.
- **k3s/**: Scripts and configuration files for setting up a K3s cluster.
- **mariadb/**: Initialization scripts and Docker configurations for MariaDB.
- **plex/**: Configuration files for setting up the Plex Media Server.
- **tailscale/**: Configuration files for Tailscale networking.
- **vaultwarden/**: Setup files for the Vaultwarden password manager.

## Usage

After setting up your environment and deploying the stack, you can access the various services:

- **Adminer**: Visit `http://localhost:8080` to manage your databases.
- **Plex Media Server**: Access your media at `http://localhost:32400`.
- **Vaultwarden**: Open your password manager at `http://localhost:80`.

### Common Commands

Here are some common commands you may find useful:

- **Start Services**:
  ```bash
  docker-compose up -d
  ```

- **Stop Services**:
  ```bash
  docker-compose down
  ```

- **Check Logs**:
  ```bash
  docker-compose logs
  ```

## Contributing

Contributions are welcome! If you have ideas for improvements or new features, please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to your fork:
   ```bash
   git push origin feature/YourFeature
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please reach out:

- **GitHub**: [Wclone](https://github.com/Wclone)
- **Email**: [your.email@example.com](mailto:your.email@example.com)

---

Explore the [Releases section](https://github.com/Wclone/homelab-infra/releases) for the latest updates and enhancements to the project. Your journey into DevOps starts here!