# Category Field

## Default category field mapping

# TODO - DELETE THIS LINE - EXAMPLE

Mapped Field | #TODO Event Field | Example value
------------ | ----------------------- | -------------
exploits | `exploits` | 1
id | `id` | s3jd0xad-cb69-47dc-9bd1-nckd8eu9dwsk-default-asset-8888
last_scan | `last_scan_end` | 09/06/23 20:54:05 MDT
os_arch | `os_architecture` | x86_64
os_description | `os_description` | Microsoft Windows Server 2016 Standard Edition 1607
os_family | `os_family` | Windows
os_name | `os_name` | Windows Server 2016 Standard Edition
os_system_name | `os_system_name` | Microsoft Windows
os_type | `os_type` | Server
os_vendor | `os_vendor` | Microsoft
os_version | `os_version` | 1607
policies_assessed | `assessed_for_policies` | false
risk_score | `risk_score` | 18342.296875
tags | `tags{}.type` + `tags{}.name`| SITE: #TODO insight agents
type | `type` | guest
vuln_assessed | `assessed_for_vulnerabilities` | true
vuln_critical | `critical_vulnerabilities` | 13
vuln_moderate | `moderate_vulnerabilities` | 2
vuln_severe | `severe_vulnerabilities` | 92
vuln_total | `total_vulnerabilities` | 107
splunk_last_update | n/a | 08/26/22 18:54:42 MDT

### Full example of category value

```yaml
exploits: 1
gen: sa-#TODO
id: s3jd0xad-cb69-47dc-9bd1-nckd8eu9dwsk-default-asset-8888
last_scan: 09/06/23 20:54:05 MDT
os_arch: x86_64
os_description: Microsoft Windows Server 2016 Standard Edition 1607
os_family: Windows
os_name: Windows Server 2016 Standard Edition
os_system_name: Microsoft Windows
os_type: Server
os_vendor: Microsoft
os_version: 1607
policies_assessed: false
risk_score: 18342.296875
splunk_last_updated: 09/06/23 21:40:30 MDT
tags: SITE: #TODO insight agents
type: guest
vuln_assessed: true
vuln_critical: 13
vuln_moderate: 2
vuln_severe: 92
vuln_total: 107
```