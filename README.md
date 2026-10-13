# Awesome-Field-Audit-Trail-History

# Top Field Audit Trail & History Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Field-Level Change Tracking, Data Retention & Compliance Archiving*
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Field Audit Trail & History**. These tools enable organizations to track field-level changes, maintain long-term audit trails for compliance (SOX, HIPAA, GDPR, 21 CFR Part 11), and archive historical data for forensic investigations—ensuring data integrity and regulatory readiness.

**Examples** include Salesforce Shield Field Audit Trail, OwnBackup Archive (Own Archive), Odaseva Data Retention, GRAX, Flosum Audit Trail, AutoRABIT Vault, Keepit Archive, Veeam Archive, Spanning Archive, and Commvault Cloud (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, cryptographic audit integrity, and open archival infrastructure—ideal for compliance officers, IT teams, and developers seeking transparent, vendor-independent audit trail solutions.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Salesforce Shield Field Audit Trail](https://help.salesforce.com/s/articleView?id=platform.shield_ext_history_retention.htm&type=5)**
  Extends field history retention from standard 18 months to up to 10 years . History Retention Policy Manager provides centralized view of all supported objects with history tracking, archive schedules (0-18 months), retention periods (0-10 years), and grace periods (0-10 days) . Automated visual indicators identify sensitive fields. Supports up to 20 custom fields plus 60 standard fields per object. Critical for SOX, HIPAA, and forensic investigations .

- **[Own Archive (formerly OwnBackup)](https://www.ccrm.philips.ru/eu/platform/own-integration/)**
  Ranked #1 Enterprise SaaS Backup by G2, now part of Salesforce Agentforce 360 Platform. 65 billion+ records archived to date . Tailor retention policies per instance with daily backups retained up to 10 years and monthly backups up to 99 years . Searchable archives of historical data support keyword searches across backups, files, and attachments for audit readiness .

- **[Odaseva Data Retention](https://www.odaseva.com/)**
  Enterprise Salesforce data protection with automated backup, restore, archiving, and sandbox anonymization . Service NSW uses Odaseva to enforce 2, 5, 7, and 10-year retention policies across complex objects with varying retention times . Daily reports, monitoring dashboards, and instant warnings provide confidence in recovery plans .

- **[GRAX](https://www.grax.com/)**
  Bring Your Own Cloud (BYOC) data platform for Salesforce Admins and IT teams. Continuous backup of data, metadata, files, and attachments with granular and point-in-time mass recovery . Parquet Data Lake (formerly History Stream) enables data reuse beyond archiving. Global medical device company replicated 18+ TB with 100% data retention and access in their own Azure Cloud .

- **[Flosum Audit Trail](https://success.flosum.com/s/article/Export-Audit-Trail-Changes-Recorded-in-Org)**
  DevSecOps platform with complete, uneditable history of all code and component version changes . Audit Trail feature identifies unauthorized changes that did not go through Flosum, helping Compliance Officers bridge compliance gaps . Custom reports can be created to export audit trail data for external analysis.

- **[AutoRABIT Vault](https://knowledgebase.autorabit.com/)**
  Salesforce data protection with backup, archive, and GDPR compliance modules . Download files directly from backups and archives. Range-based date masking for sensitive fields. Supports Big Objects, Special Objects, and Entity Definition backups. Improved session stability during file archiving .

- **[Keepit Archive](https://www.keepit.com/)**
  Vendor-neutral cloud backup with 10-year retention guarantee . German Compliance Partners (GCP) selected Keepit for 10-year financial data retention compliance. Deleted Items View searches across historical backup datasets through time. Snapshot feature identifies exact files before restore. Single admin manages 1,500 users. No hidden costs—storage, SLAs, and 24/7 support included .

- **[Veeam Archive](https://helpcenter.veeam.com/docs/vbr/userguide/azure_cosmos_db_backup_archiving.html)**
  Backup archiving to low-cost, long-term Archive access tier . Combines daily/weekly/monthly schedules with separate archive schedules for extended retention. Minimum storage duration of Archive tier is 180 days. Restoring from archive is longer and more expensive than regular backups .

- **[Spanning Archive](https://spanning.com/)**
  SaaS data protection for Microsoft 365, Google Workspace, and Salesforce. Automated daily backups with granular restore and ransomware recovery.

- **[Commvault Cloud](https://learn.microsoft.com/en-us/azure/partner-solutions/commvault/overview)**
  Azure Native integration for immutable, air-gapped data protection . Automated and orchestrated recovery supporting rapid, granular, and mass restore. Protection against ransomware, accidental deletion, and malicious modification. Unified billing through Azure Marketplace .

## Open-Source GitHub Projects

- **[historify](https://pypi.org/project/historify/)**
  Command-line tool for revision-safe file change logging with cryptographic integrity verification . Uses BLAKE3 and SHA256 hashing with minisign signatures. Full chain verification ensures tamper-evident history. Tracks new files, modifications, moves, deletions, and administrative events. Multiple repositories and logical categorization. Particularly suited for adding compliance and audit capabilities to cloud storage systems like Nextcloud .

- **[regulog](https://cran.r-project.org/web/packages/regulog/regulog.pdf)**
  R package for regulated environment audit logging with SHA-256 hash chain integrity . Every entry stores hash of all prior entries—altering any field breaks the chain. Entry types: ACTION (discrete events), CHANGE (before/after field modifications), NOTE (free-text decisions), SIGNATURE (named sign-off). Addresses 21 CFR Part 11 and EU Annex 11 requirements with IQ/OQ/PQ validation scripts. Export to CSV or JSON with optional signing. Works offline from raw .rlog files .

### Additional Strong Open-Source Options

- **[Apache Atlas](https://github.com/apache/atlas)** — Open-source metadata and governance (Apache-2.0) with lineage tracking and audit capabilities.
- **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** — Open-source metadata platform (Apache-2.0) with change events and audit logs.
- **[DataHub](https://github.com/datahub-project/datahub)** — Open-source metadata platform (Apache-2.0) with timeline and audit trail features.
- **[Nextcloud](https://github.com/nextcloud/server)** — Open-source file sync (AGPL-3.0) with activity tracking and audit logging.
- **[Auditd](https://github.com/linux-audit/audit-userspace)** — Linux kernel audit subsystem for system-level change tracking.
- Community **n8n** workflows for audit trail export automation and compliance reporting.

**Frameworks for building custom systems**: Combine **historify** for cryptographic file change logging with **regulog** for regulated environment audit trails, **Apache Atlas** or **DataHub** for metadata lineage and governance, and **PostgreSQL** for persistence—creating a fully self-hosted, enterprise-grade audit trail and history platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Audit trail and history systems handling regulated data must comply with industry-specific regulations (SOX, HIPAA, GDPR, 21 CFR Part 11, etc.).
- Self-hosted open-source solutions require proper cryptographic key management, secure storage, and ongoing maintenance. Field Audit Trail is critical for detecting unauthorized data modifications and insider threats—without it, organizations lose their primary mechanism for detecting systematic data tampering .

---

**Made for compliance officers, Salesforce administrators, IT governance teams, and developers building transparent audit trail solutions.**
Let's make Field Audit Trail & History more open, data-driven, and auditable.
