# Asset Database Mapping

# TODO - DELETE THIS LINE - Example

The following table describes how this add-on maps to the Asset Database.

> reference [Format an asset or identity in Splunk ES<small>:icon-link-external:</small>](https://docs.splunk.com/Documentation/ES/latest/Admin/Formatassetoridentitylist#Asset_lookup_header){ target="blank" }

ES Asset lookup field | [#TODO InsightVM TA Fields<small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/#TODO){ target="blank" } | Example value | Multi-value allowed
--- | --- | --- | ---
ip | `ip` | 10.15.23.8 | true
mac | `mac` | 61:se:e3:1s:7r:38 | true
nt_host | `host_name` | dev-server01 | false
dns | `hostname` | dev-server01.example.com | true
owner | n/a | `not mapped` | n/a
priority | see [Configure Priority](../configure/priority.md) | medium | false
lat | n/a | `not mapped` | n/a
long | n/a | `not mapped` | n/a
city | n/a | `not mapped` | n/a
country | n/a | `not mapped` | n/a
bunit | n/a | `not mapped` | n/a
category | see [Category field reference](category.md) | see [Category field reference](category.md) | true
pci_domain | n/a | `not mapped` | n/a
is_expected | n/a | `not mapped` | n/a
should_timesync | n/a | `not mapped` | n/a
should_update | n/a | `not mapped` | n/a
requires_av | n/a | `not mapped` | n/a
cim_entity_zone | n/a | `not mapped` | n/a