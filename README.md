# nginx_efk_stack
# Elasticsearch-Filebeat-Kibana Stack for Monitoring Nginx Logs

## Overview

This project sets up an Elasticsearch-Filebeat-Kibana stack to monitor and visualize Nginx access and error logs. The stack consists of the following components:

- **Nginx**: A web server that serves the application and generates access and error logs.
- **Elasticsearch**: A search and analytics engine that stores and indexes the logs.
- **Filebeat**: A lightweight shipper for forwarding and centralizing log data, which streams Nginx logs to Elasticsearch.
- **Kibana**: A data visualization tool that allows users to interact with the data stored in Elasticsearch.

## How It Works

- Nginx access and error logs are written to a designated directory, which is mapped to a local volume.
- Filebeat reads the Nginx logs from the local volume and sends them to an Elasticsearch index named `filebeat-*`.
- Kibana uses the Elasticsearch index to visualize the access and error logs, providing insights and analytics.

## Prerequisites

Before running the stack, ensure you have the following installed:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Getting Started

To run the Elasticsearch-Filebeat-Kibana stack, follow these steps:

1. Clone this repository or download the project files to your local machine.
2. Navigate to the project directory.
3. Execute the following command to start the stack:

   ```bash
   docker-compose up -d
   
# Images

![Screenshot from 2024-09-28 10-55-44](https://github.com/user-attachments/assets/50d12bd3-a82b-4de0-8674-336254afab93)
![Screenshot from 2024-09-28 10-55-41](https://github.com/user-attachments/assets/7d0e1472-fde2-4b0d-b0fc-51a49db4d1f8)

