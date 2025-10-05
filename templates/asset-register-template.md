# Asset Register Template

Use this register to maintain an inventory of information assets, infrastructure components, and critical services. Align asset classifications with the Information Security Policy.

| Asset ID | Asset Name / Description | Asset Type (Hardware / Software / Data / Service) | Owner (Role / Department) | Custodian / Support Team | Information Classification | Vulnerability Score (CVSS / Internal) | Location / Hosting | Business Criticality | Dependencies | Backup / Recovery Details | Last Review Date |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |

## Asset Lifecycle Notes

| Asset ID | Event (Acquisition / Update / Decommission) | Description | Date | Authorised By |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
|  |  |  |  |  |

> **Reminder:** Link this register to configuration management databases (CMDBs) and update risk assessments when asset criticality changes.

## Sorting and Filtering Tips

- **Sort by critical attributes:** Apply sorting on the Asset ID, Owner, or Vulnerability Score columns to quickly prioritise review work. In spreadsheets, highlight the table and enable *Filter* to add dropdowns for each column.
- **Filter by classification:** Use the Information Classification filter to focus on Highly Sensitive or Restricted assets during targeted assessments.
- **Create priority views:** Combine filters (for example, Classification = "Confidential" and Vulnerability Score ≥ 7) to surface remediation candidates.

## Importing from CSV (Example)

If your asset discovery tools export CSV files, create a simple import sheet to paste raw data before copying into the register. Example CSV layout:

```csv
Asset ID,Asset Name,Asset Type,Owner,Custodian,Classification,Vulnerability Score,Location,Business Criticality,Dependencies,Backup Details,Last Review Date
AS-001,Customer Database,Data,Data Protection Lead,DBA Team,Confidential,8.2,Primary Data Centre,High,CRM Platform;Analytics Warehouse,Nightly full backup,2024-06-15
AS-002,Web Gateway,Service,IT Operations Manager,Network Team,Internal,5.6,Cloud Edge,Medium,Firewall Cluster;Monitoring Stack,Daily config backup,2024-05-30
```

> **Tip:** When importing into spreadsheet software, ensure the Vulnerability Score column is set to numeric format so that conditional formatting and sorting work correctly.
