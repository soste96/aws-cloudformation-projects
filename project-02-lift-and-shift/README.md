# Project 02 — Lift & Shift EC2 Migration

## What I Built
Simulated an on-premises to AWS cloud migration using a 
Lift-and-Shift strategy — no code changes, no rebuilding 
from scratch. Captured a full server snapshot and used it 
to deploy an identical server in the cloud.

## Architecture
- **EC2 Instance #1** (onprem-server) — simulated the original 
  on-premises server running Apache web server
- **AMI (onprem-app-v1)** — full snapshot of the original server 
  capturing OS, software, and configuration
- **EC2 Instance #2** (cloud-migrated-server) — new cloud server 
  launched directly from the AMI with zero manual configuration

## Migration Steps
1. Launched EC2 instance simulating on-premises server
2. Installed Apache and deployed web application manually
3. Created AMI snapshot of the configured server
4. Launched new EC2 instance from AMI in the cloud
5. Verified identical application running on new server
6. Terminated original instance and cleaned up all resources

## Before vs After
| | Before (On-Premises) | After (AWS Cloud) |
|---|---|---|
| Hardware | Physical/fixed | EC2 on demand |
| Provisioning | Manual setup | AMI-based instant deploy |
| Capacity | Fixed | Scalable |
| Cost | Always on | Pay as you go |
| Recovery | Slow | Relaunch from AMI |

## Key Concepts Demonstrated
- AMI creation and deployment
- EC2 instance provisioning
- Lift-and-Shift migration strategy
- AWS Free Tier cost management
- Resource cleanup (EC2, AMI, Snapshots)

## Result
Two different IP addresses serving identical applications —
proving a successful migration from simulated on-premises 
infrastructure to AWS cloud with zero application changes.
