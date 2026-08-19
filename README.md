# Project 7 – Monitoring DevOps Applications Using Prometheus and Grafana

## ?? Project Overview

This project demonstrates how to monitor DevOps applications and Windows system resources using Prometheus, Windows Exporter, and Grafana.

Prometheus collects and stores metrics, Windows Exporter exposes Windows system metrics, and Grafana provides visualization through a monitoring dashboard.

## ??? Architecture

Windows System
¦
?
Windows Exporter
¦
¦ Metrics :9182
?
Prometheus :9090
¦
¦ PromQL
?
Grafana :3000
¦
?
Monitoring Dashboard

## ??? Technologies Used

* Prometheus 3.13.2
* Grafana
* Windows Exporter
* PromQL
* Windows
* PowerShell

## ?? Prometheus Configuration

Prometheus is configured with a 15-second scrape interval.

### Monitored Targets

|Job|Target|Purpose|
|-|-|-|
|prometheus|localhost:9090|Prometheus self-monitoring|
|windows|localhost:9182|Windows system metrics|

## ?? Monitoring

The Grafana dashboard includes:

* Prometheus Target Status
* Prometheus Uptime
* CPU Usage
* Memory Usage
* Prometheus Scrape Duration
* Windows Exporter metrics

## ?? PromQL Example

`promql
up
????? Author

Pranjali S. Malode

