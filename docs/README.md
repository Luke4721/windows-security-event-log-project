Windows Security Event Log Investigation
Welcome! 👋
This project demonstrates a hands-on approach to detecting suspicious activities and potential threats within Windows Security Event Logs using Splunk. The goal? To surface real-world attacker behavior — like privilege misuse or RDP attack attempts — and show how a SOC analyst would hunt, visualize, and document these incidents.

🚩 Project Overview
This repository showcases:

The end-to-end workflow of ingesting large-scale Windows Event data into Splunk.

Step-by-step creation of detection SPL queries targeting privilege misuse, RDP activity, and “noisy” users or endpoints.

Clean, recruiter-friendly dashboards that highlight exactly where, when, and how suspicious activity occurred.

A detailed incident report summarizing patterns, findings, and recommended SOC actions.

Whether you’re a hiring manager, peer, or fellow analyst curious about blue-team tactics, everything here is designed to be accessible, reproducible, and robust.

📂 Repository Structure
text
/
├── data/                  # Sample Windows EVTX logs and/or processed CSVs (for reproducibility)
├── search_queries/        # All SPL queries used for investigation, ready for Splunk import
├── dashboard_screenshots/ # Key visualizations and panels created in Splunk
├── incident_report.md     # Clear summary of what was investigated, discovered, and next steps
└── README.md              # You are here!
🔎 Key Analysis Use Cases
The project answers questions every SOC analyst faces, such as:

Who are the most targeted or abused user accounts on the network?

Which IPs or devices are generating the most high-severity alerts?

Are there signs of privilege misuse, endpoint compromise, or RDP brute force?

What malware or suspicious files are being executed?

Do logins from the same account appear in impossible or risky locations?

What MITRE ATT&CK tactics and techniques are prevalent in the log sample?

📊 Dashboard Panels
The main Splunk dashboard delivers:

Bar charts for the top-impacted accounts and noisy IPs

Trend line or timechart panels for alert spikes and temporal patterns

Tables showing endpoint, file, and role-based alert breakout

MITRE technique mapping visualizations

Geo-mapping or country-based anomaly tables (for impossible travel detections)

Direct drilldowns to the raw logs for further investigation

🛠️ How to Reproduce
Ingest the EVTX or CSV log samples from /data into your local Splunk instance.

[Optional] Use the provided SPL files in /search_queries — just copy and paste into Splunk search.

Recreate the dashboard by using the sample panels (see /dashboard_screenshots for ideas).

Review or extend the provided incident_report.md for narrative or to guide your own documentation.

📜 Why This Project Matters
Understanding and visualizing attacker movement is a must for any SOC analyst job.
This project doesn't just show you can use Splunk — it proves you can think like an investigator, automate detection, and communicate findings to both technical teams and non-technical stakeholders.

Open for feedback, suggestions, and collab.
If you see ways to sharpen queries, improve the dashboard, or just want to chat blue teaming, feel free to reach out!

👤 Author
Made with real threat hunting curiosity by Yakshvardhan Jaitely.

