---
order: -3
label: Update Index
icon: command-palette
---

# Update Splunk Index

!!!danger [Danger, Will Robinson <small>:icon-link-external:</small>](https://cultural-phenomenons.fandom.com/wiki/Danger,_Will_Robinson){ target="blank" }
Failure to update the index to the correct setting will cause no threat intel to be available in Splunk Enterprise Security.
!!!

The index definition is set by a search macro. 

Macro | Default | Description
----- | ------- | -----------
`crowdstrike_intel_index` | index=crowdstrike_ioc | Index definition for CrowdStrike Intel Indicators index.

## How to update

1. Navigate to Settings > Advanced Search > Search Macros.
2. From the "App" dropdown choose `SA-CrowdstrikeIntelIndicators`.
3. Set the "Owner" dropdown to `any`.
4. Click the macro named `crowdstrike_intel_index` to update the index definition.