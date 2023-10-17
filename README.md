Nim    : 22.83.0815 - TK01

# moiOs
Alat untuk melakukan pemantauan seluruh kinerja yang sedang berlangsung pada suatu server adalah sebuah solusi yang sangat berguna. Dengan bantuan Server Monitoring, kita dapat memperoleh pemahaman mendalam tentang penggunaan sumber daya sistem, seperti pemantauan tingkat penggunaan CPU, penggunaan memori, aktivitas Input dan Output, pemantauan jaringan, penggunaan kapasitas penyimpanan disk, dan aspek-aspek lain yang terkait.
SysAdmin - project

## Daftar Isi
1. [moiOs](#moiOs)
2. [Resourece](##Resource)
3. [Service](##Service)
4. [Installation](##Installation)
5. [Configuration](##Configuration)
6. [Contribution](#Contribution)
7. [Lisence](#Lisence)

## Getting Started

Welcome to the Monitoring Server project! This project is designed to help you monitor and analyze your server's performance by tracking resource utilization such as CPU usage, memory usage, I/O activity, network activity, and more.

To get started with the Monitoring Server, follow the instructions below:

## Resource
   - Debian 11

## Service
   - Ssh
   - NetworkManager
   - Prometheus

## Installation
   **Update Package**
   ```shell
    sudo apt-get update
   ```

   **Install NetworkManager** 
   ```shell
   sudo apt -y install network-manager
   ```

   **Install ssh**
   ```shell
   apt-get install openssh-server
   ```

   **Install Prometheus**
   ```shell
   apt -y install prometheus prometheus-node-exporter
   ```

   
## Configuration
# Contribution
# Lisence
