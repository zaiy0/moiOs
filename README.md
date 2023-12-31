# moiOs
Alat untuk melakukan pemantauan seluruh kinerja yang sedang berlangsung pada suatu server adalah sebuah solusi yang sangat berguna. Dengan bantuan Server Monitoring, kita dapat memperoleh pemahaman mendalam tentang penggunaan sumber daya sistem, seperti pemantauan tingkat penggunaan CPU, penggunaan memori, aktivitas Input dan Output, pemantauan jaringan, penggunaan kapasitas penyimpanan disk, dan aspek-aspek lain yang terkait.
SysAdmin - project

## Daftar Isi
1. [moiOs](#moiOs)
2. [Resourece](#Resource)
4. [Service](#Service)
5. [Installation](#Installation)
6. [Configuration](#Configuration)
7. [Screenshot](#Screenshot)
8. [Lisence](#Lisence)

## Getting Started

Welcome to the Monitoring Server project! This project is designed to help you monitor and analyze your server's performance by tracking resource utilization such as CPU usage, memory usage, I/O activity, network activity, and more.

To get started with the Monitoring Server, follow the instructions below:

## Resource
   - Debian 12

## Service
   - SSH
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

   **Install Prometheus beserta Node Exporter**
   ```shell
   apt -y install prometheus prometheus-node-exporter
   ```

   
## Configuration 
   **Edit file konfigurasi Prometheus**
   ```shell
   vi /etc/prometheus/prometheus.yml
   ```

   **Konfigurasi untuk menargetkan Prometheus**
   ```shell
   scrape_configs:
     - job_name: 'prometheus'
       static_configs:
         - targets: ['your_server_IP:9090']
   ```

   **Tambahkan konfigurasi untuk menargetkan Node Exporter**
   ```shell
   scrape_configs:
     - job_name: 'node-exporter'
       static_configs:
         - targets: ['your_server_IP:9100']
   ```
   Jika sudah, simpan file konfigurasi tersebut
   
   **Buka Grafana di browser**
   ```shell
   http://alamat_IP:3000
   ```
   Gunakan default login:admin, password:admin

# Screenshot
   **Prometheus**
![Screenshot (516)](https://github.com/zaiy0/moiOs/assets/90432809/0853c343-0353-471b-a02e-f5be3f116974)
   **Node Exporter**
![Screenshot (515)](https://github.com/zaiy0/moiOs/assets/90432809/fdc5098d-b3ff-40f2-a9a2-591700e75eef)
   **Grafana**
![Screenshot (514)](https://github.com/zaiy0/moiOs/assets/90432809/dd1a33b6-519a-4d97-ac70-69632b641cf8)

 **Grafana Dashboard - Node Exporter Full**
 ![image](https://github.com/zaiy0/moiOs/assets/90432809/7c70597f-8c3e-4f74-97ef-2bab395aad2a)

 


# Contribution
Nim    : 22.83.0815 - TK01


# Lisence
                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/
