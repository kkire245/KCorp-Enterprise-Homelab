# KCorp Enterprise Homelab

A self-built enterprise identity environment simulating a mid-sized company (KCorp), used to develop hands-on skills in Active Directory administration, hybrid identity, and Microsoft Entra ID / IAM.

## Project Goal
Build a realistic, documented enterprise identity environment from the ground up, starting with on-prem Active Directory administration, then extending into hybrid identity and cloud IAM (Entra ID, Conditional Access, PIM, Governance). This is to develop and demonstrate real, configurable skills rather than just certification knowledge.

## Environment Overview
- **Tenant:** Microsoft Entra ID (KCorp), Entra ID P2 trial
- **On-prem:** Windows Server (Hyper-V), Active Directory Domain Services, domain: `kcorp.local`
- **Departments simulated:** IT, HR, Finance, Sales, Operations
- **Users:** 25 fictional employees across departments, mix of standard/admin/contractor accounts

## Structure
| Folder | Contents |
|---|---|
| `01-Entra-ID/` | Entra tenant setup, users, groups, licensing |
| `02-Active-Directory/` | On-prem AD: DC setup, OUs, users, groups, GPOs |
| `03-Hybrid-Identity/` | Entra Connect install/config, sync verification |
| `04-Authentication/` | MFA, SSPR, Temporary Access Pass |
| `05-Conditional-Access/` | CA policies, What If testing, report-only rollout |
| `06-PIM/` | Privileged Identity Management — eligible roles, activation, audit |
| `07-Governance/` | Access packages, entitlement management, access reviews |
| `08-Automation/` | PowerShell / Microsoft Graph scripts |
| `screenshots/` | Supporting screenshots, referenced from entries |

## Build Log
A running list of major milestones, updated as phases complete.

| Date | Milestone |
|---|---|
| Aug 2026 | Entra tenant created (KCorp), 25 users provisioned |
| Aug 2026 | Entra ID P2 trial activated |
| Aug 2026 | Hyper-V enabled |
| Aug 2026 | Windows Server 2025 evaluation ISO downloaded |
| Aug 2026 | Security groups created (5 assigned + 1 dynamic), guest user invited |
| Aug 2026 | **Phase 0 complete** |
| Aug 2026 | KCorp-DC01 built, promoted to domain controller (kcorp.local) |
| Aug 2026 | OU structure, AD users, and nested security groups created |
| Aug 2026 | 3 GPOs created and linked; client VM joined to domain and confirmed policy application |
| Aug 2026 | **Phase 1 complete** |
| | *(add entries as you go)* |

## How Entries Are Documented
Every meaningful configuration gets its own file in the relevant folder, using the template in `CONFIG-TEMPLATE.md`: what I wanted to accomplish → what I configured → why → how I tested it → result.
