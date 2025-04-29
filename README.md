# Jukebox Inc. Analytics Project

## Overview
Welcome to the Jukebox Inc. Analytics repository. This project supports the company's mission to modernize and expand the use of internet-connected jukeboxes across bars in Africa. As an analytics engineer, the goal is to transform event-sourced data into actionable insights that drive decisions across sales, finance, marketing, and operations.

## Business Context
Jukebox Inc. earns revenue through:
- An **initial installation fee** per jukebox device.
- **Royalties** based on each song played.

Devices and customer payments are tracked using event-based infrastructure, which requires precise logic to attribute events to business outcomes.

## Key Analytics Objectives
### 1. **Jukebox Sales Tracking**
- **Definition**: A jukebox is considered "sold" when allocated to a location *and* full payment (equal to or greater than `DevicePrice`) is received.
- **Challenges**:
  - Installmental Payments.
  - Multi-device Payments.
  - Internal transfers between customer locations (not sales).
  - Royalty Payments.
    

### 2. **Agent Revenue-Sharing Program**
- Identify agents whose installed devices generate the most song plays per month.
- Metrics:
  - Monthly song plays per jukebox per agent.
  - Rank agents by usage to determine incentive distribution.

### 3. **Cash Flow Analysis and Forecasting**
- **[a] Historical & Projected Cash Movements**:
  - Include income (jukebox sales, royalties) and expenses (inventory, licensing, agent payouts).
- **[b] Customer-level Reconciliation**:
  - Compare expected vs. actual payments received, by time period and customer.

### 4. **Product Launch Performance**
- Track sales and usage metrics for specific products (e.g. *MusicMaker3000*).
- Compare performance across product launches over time.
- Enable **self-service dashboards** for marketing stakeholders.


## Technologies

- **Data Warehouse**: Microsoft SQL Server
- **Data Modelling Tool**: dbdiagram.io
- **Visualization Tool**: Looker Studio
- **Version Control**: Git / GitHub

## Getting Started

1. Clone this repository.
2. Review `ER Diagram/` for dbt models.
3. See `docs/` for event definitions and logic guides.
4. Use `dashboards/` for examples of self-service analytics.


---

