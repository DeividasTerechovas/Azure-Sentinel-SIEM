# Azure-Sentinel-SIEM

# Brute Force Attack Detection with Azure Sentinel

# Objective

The project focused on configuring Microsoft Sentinel, a cloud-native Security Information and Event Management (SIEM) system, to detect and respond to brute force attacks. The goal was to simulate real-world attack scenarios within a controlled environment, analyze security logs, and generate alerts for unauthorized access attempts.

# Skills Learned

Deployment and configuration of Microsoft Sentinel.

Log aggregation and analysis using Azure Log Analytics.

Recognizing and responding to brute force attack patterns.

Integration of threat intelligence feeds to enhance detection capabilities.

Hands-on experience in real-time security event monitoring.

# Tools Used

Microsoft Sentinel – Cloud-native SIEM for log aggregation and threat detection.

Azure Log Analytics – Collects and presents security logs.

Virtual Machines (Windows Server) – Used as monitored endpoints.

Threat Intelligence Feeds – For automated consumption of the latest Indicators of Compromise (IOCs).

Telemetry Generation Tools – To simulate attack scenarios.

# Steps

1. Setting Up Azure Sentinel

Signed up for an Azure account (free version available with $200 credit).

Created a Log Analytics Workspace and deployed Microsoft Sentinel.

2. Deploying and Configuring a Virtual Machine

Set up a Windows Server Virtual Machine.

Opened port 3389 to attract unauthorized RDP login attempts.

Installed Azure Monitor Agent (AMA) to send security logs to Sentinel.

3. Configuring Log Collection & Threat Detection

Connected the VM logs to Azure Sentinel.

Enabled security event collection, specifically monitoring failed RDP login attempts.

Integrated threat intelligence feeds to enhance detection.

4. Monitoring and Analyzing Attacks

Observed brute-force attempts within 24 hours.

Identified attack sources, primarily from Russia and North Korea.

Automated detection and alerting of repeated intrusion attempts.

5. Response & Automation

Implemented alert rules to detect failed login attempts.

Configured playbooks to trigger automated responses.

Simulated SOC analyst activities by analyzing logs and crafting incident reports.

Real-World Observations

Attackers began scanning open RDP ports almost immediately after exposure.

Hundreds of brute-force attempts were detected daily.

Microsoft Sentinel effectively flagged repeated unauthorized login attempts.

# Why This Matters

Mimics real-world SOC operations – Hands-on Blue Team training.

Enhances cybersecurity skills – Practical SIEM deployment experience.

Improves defensive strategies – Learn how attackers probe RDP ports and how to mitigate them.

# Screenshots & References


https://imgur.com/a/J7Wm8GA

First image shows the data we collected

https://imgur.com/a/gvYN1BU

Second image shows us using KQL to search for important information from the 24h period

https://imgur.com/a/FV3eVPE

This 3rd image provides data on succesfull attacks done to our virtual machine
