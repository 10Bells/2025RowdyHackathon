2025 RowdyHackathon
# Windows Event Log SIEM using Splunk

## Overview
A lightweight SIEM solution built on Splunk Enterprise to detect failed logins, brute-force attempts, and suspicious authentication patterns.

## Features
- Real-time monitoring of Windows Security logs
- Custom Splunk alerts for brute-force and suspicious logins
- Dashboard visualizations for security events

## How it works
1. Splunk collects local Windows Security Event Logs (EventCode 4624, 4625)
2. SPL queries detect patterns (failed→success logins, excessive failures)
3. Alerts trigger email notifications and event logging

search/
{
   alerts/
    {
      Brute_Force_Attempt_alert.spl (2 more fails)
      Suspicious_Login_ Detected_alert.spl (incorrect-> sucessful login)      
   }
   dashboards/
   {
      Security_Monitoring_&_Incident_Dashboard.png
   }
}
