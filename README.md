Splunk Blue Team Lab – Advanced SIEM Use Case

A fully operational Splunk lab built for blue teamers, SOC analysts, and cybersecurity engineers.

🏗️ Features

- Ingestion of Windows & Linux logs via Universal Forwarder
- Real-time dashboards for failed logins and geo activity
- Alerts for brute-force, admin logins, and threat matches
- Index management (retention, filtering, summary indexing)
- Threat intelligence integration via custom lookup tables

📂 Folder Structure

- `dashboards/`: Ready-to-import XML dashboards
- `alerts/`: SPL queries for real-time detection
- `configs/`: `props.conf`, `transforms.conf`, `indexes.conf`
- `lookups/`: CSV files for threat intel and IP geolocation
- `summary_indexing/`: Summary indexing queries
- `sample_logs/`: Auth logs and synthetic data

📊 Dashboards

- `login_monitoring.xml`: Failed logins, top sources
- `threat_intel_dashboard.xml`: Matches from threat lookup
- `index_volume.xml`: Storage monitoring

📢 Alerts

- Brute-force SSH (failed logins > 5)
- Admin logins on Windows
- Login from foreign country
- Threat IP match

🔧 Index Management

- `frozenTimePeriodInSecs` for retention
- NullQueue for dropping DEBUG logs
- Summary indexing to reduce long-term storage


🔐 Built by [MindSec (Mohamed Basil)] – Cybersecurity & Blue Team Engineer  
🔗 Medium Blog: https://medium.com/@Mindsec/operationalizing-splunk-for-blue-team-success-from-ingestion-to-threat-detection-cdd584e29c66 
📫 Connect: www.linkedin.com/in/mohamed-basil-966a8225a
