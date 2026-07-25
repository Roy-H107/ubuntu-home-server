# 🏠 Ubuntu Home Server

Enterprise-style Ubuntu Server homelab featuring Docker, Portainer, Jellyfin, Samba, Cloudflare DDNS, and dedicated game server hosting.

---

![Ubuntu](https://img.shields.io/badge/Ubuntu-26.04_LTS-E95420?logo=ubuntu&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-DDNS-F38020?logo=cloudflare&logoColor=white)
![TCPShield](https://img.shields.io/badge/TCPShield-Game_Protection-6E56CF)
![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?logo=docker&logoColor=white)
![Jellyfin](https://img.shields.io/badge/Jellyfin-Streaming-00A4DC)
![Samba](https://img.shields.io/badge/Samba-File_Sharing-008000)

---

# 📖 Overview

I built this Ubuntu Server homelab to become comfortable with Linux while creating infrastructure that provides real value to the people around me.

Rather than building a lab solely for learning, I wanted to create services that I would actually use every day. This project has grown into a platform for media streaming, file sharing, and dedicated game hosting for friends and family.

One of my favorite moments was successfully hosting a Palworld server that supported seven players at once. Seeing people actively use something I built reinforced that the best way to learn infrastructure is by solving real problems for real users.

Throughout this project I gained hands-on experience with Linux administration, networking, Docker containerization, firewall configuration, storage management, DNS, and troubleshooting by building, breaking, and continuously improving a production-style home server.

---

# 💭 Why I Built This

When I started this project, my biggest concern was ending up with a complicated environment that I didn't understand.

I wanted to avoid blindly following tutorials and instead learn how each component worked so I could confidently troubleshoot issues, explain the architecture, and maintain it over time.

Every service added to this server became an opportunity to better understand Linux, networking, Docker, and systems administration through hands-on experience.

---

# 🏗️ System Architecture

```text
                        Internet
                            │
                      Cloudflare DDNS
                            │
                     Xfinity Gateway
                            │
                     Port Forwarding
                            │
                       UFW Firewall
                            |
                ┌─────────────────────────┐
                │     Ubuntu Server       │
                │      HP Victus 15       │
                └─────────────────────────┘
                            │
                       Docker Engine
           ┌────────────────┼─────────────────┐
           │                │                 │
       Portainer        Jellyfin      Palworld Server
                            │
                          Samba
                            │
            Windows PCs • Smart TVs • Friends
```

# 🎯 Objectives

- Learn Linux administration
- Deploy containerized applications using Docker
- Manage containers with Portainer
- Configure secure network services
- Host dedicated game servers
- Centralize media with Jellyfin
- Configure Samba network shares
- Practice infrastructure documentation

---

# 🖥️ Hardware

| Component | Specification |
|------------|--------------|
| System | HP Victus 15 |
| CPU | AMD Ryzen 5 8645HS |
| Memory | 32 GB DDR5 |
| GPU | NVIDIA RTX 4050 |
| Storage | 500 GB NVMe SSD |
| Operating System | Ubuntu Server 26.04 LTS |

---

# 🧰 Software Stack

| Technology | Purpose |
|------------|---------|
| Ubuntu Server | Operating system |
| Docker | Containerization platform |
| Portainer | Docker management interface |
| Jellyfin | Self-hosted media server |
| Samba | Network file sharing |
| Cloudflare DDNS | Dynamic DNS management |
| SSH | Remote administration |
| UFW | Host firewall |
| Palworld Dedicated Server | Multiplayer game hosting |

---

# 🛠️ Services

| Service | Purpose |
|----------|---------|
| Docker | Container platform |
| Portainer | Docker management |
| Jellyfin | Media streaming |
| Samba | Network file sharing |
| Cloudflare DDNS | Dynamic DNS |
| Palworld Server | Dedicated game server |

---

# 🧠 Design Decisions

## Why Ubuntu Server?

I chose Ubuntu Server because I wanted to become comfortable with Linux in an environment commonly used for servers and infrastructure.

## Why Docker?

Docker allowed me to isolate applications into individual containers, making deployment, updates, and troubleshooting significantly easier than installing services directly on the operating system.

## Why Portainer?

Portainer provides a clean web interface for managing Docker containers while still allowing me to learn Docker's command-line tools.

## Why Jellyfin?

I wanted a self-hosted media server that I owned and controlled without subscription fees.

## Why Samba?

Samba allowed Windows devices on my network to access centralized media and shared files.

## Why Cloudflare DDNS?

My home internet connection uses a dynamic public IP address.

Cloudflare DDNS automatically updates my DNS records whenever my public IP changes, allowing me to reliably access services without manually updating DNS records.

## Why UFW?

UFW provided a simple way to manage firewall rules while limiting network exposure to only the required services.

---

# 💡 Skills Demonstrated

- Linux Administration
- Docker
- Container Networking
- Samba
- SSH
- Firewall Configuration (UFW)
- Cloudflare DNS
- Port Forwarding
- Network Troubleshooting
- Infrastructure Documentation

---

# 🚀 Future Improvements

- Reverse Proxy
- SSL Certificates
- Monitoring & Alerting
- Automated Backups
- Additional Docker Services
- Infrastructure Diagrams
- Network Topology Documentation
