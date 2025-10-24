# 🚀 NetWatch-Cloud — Real-Time Cloud Network Traffic Visualizer

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg?logo=python&logoColor=white)  
![Tool](https://img.shields.io/badge/Network-Visualizer-FF5252.svg?logo=network)  
![Features](https://img.shields.io/badge/Features-Traffic%20Charts-4CAF50.svg?logo=chart-pie)  
![Reports](https://img.shields.io/badge/Reports-PNG-2196F3.svg?logo=image)  
![CI/CD](https://img.shields.io/badge/CI/CD-Ready-2088FF.svg?logo=githubactions)  
![Dependencies](https://img.shields.io/badge/Dependencies-Matplotlib-green.svg?logo=python)

**NetWatch-Cloud** is a **Python 3** tool designed to take simulated network traffic data from multiple interfaces in a cloud infrastructure, then generate clear visual charts for inbound/outbound bytes over a series of days. It’s built for cloud engineers, network ops teams and infrastructure monitoring folks wanting quick insight into network throughput trends.

-----

## 🛠 Tech & Languages

| Layer        | Tech / Format                | Purpose                                     |
|--------------|------------------------------|---------------------------------------------|
| Language     | **Python 3.10+**             | Main codebase                               |
| Core Logic   | JSON parsing + Matplotlib     | Load traffic data, generate visualization    |
| Reports      | **PNG Image**                | Chart output for review or dashboards        |
| Execution    | Script / Colab / Notebook    | Flexible environment                        |
| Logging      | Console output + image file  | Quick summary + persisted chart              |

---

## 🌐 Architecture

Flow:  
1. Step 1 – Load `traffic_data.json` with daily in/out bytes per interface  
2. Step 2 – For each interface, sort data by date and extract in/out values  
3. Step 3 – Plot line charts (In vs Out) for each interface using Matplotlib  
4. Step 4 – Save the visualization as `traffic_chart.png` and display inline in Colab  

---

## ▶️ Run NetWatch-Cloud

```bash
python netwatch_cloud.py --input data/traffic_data.json --output data/traffic_chart.png
