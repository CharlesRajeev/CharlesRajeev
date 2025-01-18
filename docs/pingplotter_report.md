# PingPlotter Diagnostic Report

## Overview
This report details the network latency and packet loss analysis performed using PingPlotter. The goal was to simulate network issues and observe the impact on latency and packet loss.

## Key Activities

### 1. Simulate Network Latency
- **Target Selection**:
  - Enter the IP address or domain name of a target (e.g., `google.com`).
  - Start tracing the route.
- **Simulate Issues**:
  - Disconnect the internet connection or create high bandwidth usage.
  - Observe the changes in latency and packet loss.

### 2. Analyze Latency and Packet Loss
- **Latency Analysis**:
  - Identify hops with high latency.
  - Look for patterns indicating network congestion.
- **Packet Loss Analysis**:
  - Identify hops with packet loss.
  - Determine the cause of packet loss (e.g., network congestion, hardware issues).

## Screenshots and Analysis
### Normal Network Conditions
![Normal Conditions](../assets/screenshots/pingplotter_normal.png)
- **Observations**:
  - Low latency and no packet loss at all hops.

### Simulated Network Issues
![Simulated Issues](../assets/screenshots/pingplotter_simulated.png)
- **Observations**:
  - High latency and packet loss at specific hops.
  - Identified the hop causing the issue.

