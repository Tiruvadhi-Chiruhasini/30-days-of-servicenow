# Day 2 — CMDB, Configuration Items & SLAs

**Date:** 31/05/2026

## Today's Goal

Understand what CMDB is, why Configuration Items matter, and how SLAs work behind the scenes in ServiceNow.

## What I Learned

### CMDB

CMDB is basically the central inventory of an organization's IT environment. Instead of tracking products in a warehouse, it tracks things like servers, laptops, applications, databases, and network devices.

Every item stored in the CMDB is called a **Configuration Item (CI)**.

### Configuration Items (CIs)

A CI represents one real-world asset or service.

Examples:

* Laptop
* Server
* Application
* Network Device
* Database

Each CI belongs to a class, which tells ServiceNow what type of item it is.

### Relationships

One interesting thing about CMDB is that CIs are connected.

For example:

Application → Runs on Server → Connected to Network Device

These relationships help teams understand what could be affected when something fails.

### SLAs

I explored SLA definitions and understood that ServiceNow automatically tracks response and resolution deadlines.

When an incident is created, an SLA can automatically attach based on conditions like:

* Priority
* Assignment Group
* Category

If the issue isn't resolved within the target time, the SLA breaches and can trigger escalations.

## Key Terms

* **CMDB** → Database containing IT assets and services
* **CI (Configuration Item)** → A single asset or service record
* **CI Class** → Category of the CI
* **Relationship** → Connection between CIs
* **SLA** → Time commitment for handling tickets
* **Breach** → Missing the SLA deadline
* **Condition Builder** → Tool used to create filter logic with AND/OR conditions

## Biggest Takeaway

What looked like a simple incident ticket yesterday is actually connected to a much larger system.

A ticket can be linked to a Configuration Item, that CI can be connected to other CIs through relationships, and SLAs quietly track whether support teams are meeting their deadlines.

Everything in ServiceNow seems designed to connect information rather than store isolated records.

## What Surprised Me

I was surprised by how much automation happens in the background.

Creating an incident feels simple from the user side, but ServiceNow is simultaneously tracking assets, relationships, priorities, assignment rules, and SLA timers without requiring manual effort.

t before making production changes
