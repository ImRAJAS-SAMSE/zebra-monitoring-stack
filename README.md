# Zebra Monitoring Stack 🧭

A performance monitoring and observability setup for the Zebra project, integrating **Prometheus v2.30.3**, **Grafana v8.2.2**, and **MySQL** (manual installation) to support archival metrics, dashboards, and RMF MON III-style visualizations.

> ⚙️ Designed and configured as part of the Open Mainframe Project's z/OS Performance Monitoring Mentorship (Summer 2025).

---

## 📌 Features

- Manual MySQL setup for data archival and Zebra device reporting
- Integration of Prometheus as a time-series metrics collector
- Custom Grafana dashboard using mentor-provided metrics
- Replacement of default `metrics.json` with enhanced Zebra metrics
- Support for RMF MON III-type metrics for enterprise-style monitoring

---

## 🛠️ Technologies Used

| Tool         | Version    | Purpose                            |
|--------------|------------|------------------------------------|
| Zebra        | Custom     | Open Mainframe telemetry tool      |
| Prometheus   | 2.30.3     | Metrics collection                 |
| Grafana      | 8.2.2      | Metrics visualization              |
| MySQL        | 8.0+       | Report caching and archival        |
| Node.js      | 18+        | Zebra backend runtime              |

---

## 📂 Project Structure

```bash
zebra-monitoring-stack/
├── zebra_config/
│   ├── zconfig.json        # Manual MySQL and Prometheus config
│   ├── metrics.json        # Custom Zebra metrics (vinnie3.1.json)
├── dashboard/
│   └── RMF-Mon3-Grafana.json  # Pre-built Grafana dashboard
├── prometheus/
│   └── prometheus.yml      # Prometheus configuration file
├── README.md
└── ...
