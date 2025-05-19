# **ThreatViz: Cybersecurity Threat Intelligence Dashboard**

## **Overview**
**ThreatViz** is a Python-based cybersecurity threat intelligence dashboard designed to empower analysts with actionable insights through interactive data visualization. Utilizing **Matplotlib**, the application parses intrusion detection logs (e.g., Snort, Suricata), classifies threats, and generates dynamic visual reports to identify attack vectors, severity levels, and anomalies with clarity and precision.

## **Key Features**
- 📊 **Dynamic Threat Visualization**: Supports both real-time and batch processing modes.
- 📈 **Versatile Charts**: Generate bar graphs, line plots, pie charts, and heatmaps using **Matplotlib**.
- 🗂️ **Log Ingestion & Parsing**: Compatible with Snort and Suricata output formats.
- 🌍 **GeoIP Resolution**: Track and map attacker origins using IP geolocation.
- 🧩 **Modular Architecture**: Built on **Flask**, allowing seamless customization and extension.
- 🔌 **Scalable Integration**: Easily extend to support additional data sources, dashboards, or analytics tools.

## **Project Structure**
```plaintext
threatviz/
├── app/
│   ├── visualizer.py        # Handles Matplotlib chart rendering
│   ├── data_parser.py       # Parses and classifies threat logs
│   ├── routes.py            # Defines Flask application routes
│   ├── models.py            # ORM/SQLite data modeling and queries
│   ├── utils.py             # Utility functions (e.g., GeoIP, formatting)
│   └── templates/           # Jinja2 HTML templates for UI
├── datasets/                # Sample or ingested threat data logs
├── tests/                   # Unit and integration test cases
├── notebooks/               # Jupyter notebooks for EDA and prototyping
├── run.py                   # Main application entry point
├── config.py                # Central configuration settings
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
