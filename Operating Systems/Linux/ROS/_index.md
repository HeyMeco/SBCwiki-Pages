---
weight: 4
title: ROS
icon: ROS-Logo.png
iconBg: "#15253E"
summary: Robot Operating System - a flexible framework for writing robot software on ARM-based SBCs
categories:
- os
---
![ROS Logo](ROS-Logo.png?w=400&bc=15253E)

# ROS (Robot Operating System)

[Official Website](https://www.ros.org/)

## Description

ROS (Robot Operating System) is an open-source meta-operating system for robots. While not a traditional operating system, ROS provides services you would expect from an OS including hardware abstraction, low-level device control, implementation of commonly-used functionality, message-passing between processes, and package management.

ROS is widely used in robotics research and development, and is particularly popular on ARM-based Single Board Computers due to their small form factor, low power consumption, and sufficient computing power for robotic applications.

## ROS Versions

### ROS 2 (Recommended)

ROS 2 is the current actively developed version with significant improvements over ROS 1:

| Distribution | Release Date | EOL | Ubuntu Version |
|--------------|--------------|-----|----------------|
| **Jazzy Jalisco** | May 2024 | May 2029 | Ubuntu 24.04 |
| **Iron Irwini** | May 2023 | Nov 2024 | Ubuntu 22.04 |
| **Humble Hawksbill** | May 2022 | May 2027 | Ubuntu 22.04 |

**Key improvements in ROS 2:**
- Real-time capabilities
- Multi-robot systems support
- Improved security
- DDS-based communication
- Better embedded systems support
- Native support for ARM architectures

### ROS 1 (Legacy)

| Distribution | Release Date | EOL | Ubuntu Version |
|--------------|--------------|-----|----------------|
| **Noetic Ninjemys** | May 2020 | May 2025 | Ubuntu 20.04 |

> [!WARNING]
> **Note:** ROS 1 Noetic reached End of Life in May 2025. New projects should use ROS 2.

## Installation on SBCs

### Prerequisites

- Ubuntu 22.04 or 24.04 (recommended for ROS 2)
- At least 2GB RAM (4GB+ recommended)
- 16GB+ storage space
- ARM64 (aarch64) architecture

### Installing ROS 2 Jazzy on Ubuntu 24.04

```bash
# Set locale
sudo apt update && sudo apt install locales
sudo locale-gen en_US en_US.UTF-8
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
export LANG=en_US.UTF-8

# Setup sources
sudo apt install software-properties-common
sudo add-apt-repository universe
sudo apt update && sudo apt install curl -y
sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null

# Install ROS 2
sudo apt update
sudo apt install ros-jazzy-desktop  # Full desktop install
# OR
sudo apt install ros-jazzy-ros-base  # Minimal install (recommended for SBCs)

# Source the setup script
echo "source /opt/ros/jazzy/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

## Common ROS Packages for SBCs

| Package | Description |
|---------|-------------|
| `ros-<distro>-ros-base` | Minimal ROS 2 installation |
| `ros-<distro>-desktop` | Full desktop installation with visualization tools |
| `ros-<distro>-navigation2` | Navigation stack for mobile robots |
| `ros-<distro>-slam-toolbox` | SLAM (Simultaneous Localization and Mapping) |
| `ros-<distro>-image-transport` | Image transport for cameras |
| `ros-<distro>-cv-bridge` | OpenCV integration |
| `ros-<distro>-lidar-*` | Various LiDAR drivers |

## Performance Tips for SBCs

1. **Use `ros-base` instead of `desktop`** - Saves storage and RAM by excluding visualization tools
2. **Enable swap** - ROS compilation can be memory-intensive
3. **Use SSD storage** - Faster compilation and package installation
4. **Cross-compile for production** - Build on a more powerful machine, deploy to SBC
5. **Use Docker** - Pre-built ROS containers are available for ARM64

## Docker Installation (Alternative)

```bash
# Install Docker
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker $USER

# Run ROS 2 Jazzy container
docker run -it --rm ros:jazzy-ros-base
```

## Related Resources

- [ROS 2 Documentation](https://docs.ros.org/en/rolling/)
- [ROS Discourse Community](https://discourse.ros.org/)
- [ROS Answers](https://answers.ros.org/)
- [ROS on Raspberry Pi](https://docs.ros.org/en/humble/How-To-Guides/Installing-on-Raspberry-Pi.html)

## Supported Boards

ROS 2 officially supports ARM64 (aarch64) architecture and runs on most SBCs with Ubuntu support. Which can be achieved via Canonical Ubuntu Certified hardware or via Armbian.
