---
order: -3
label: Update Index
icon: command-palette
---

# Update Splunk Index

!!!danger [Danger, Will Robinson<small>:icon-link-external:</small>](https://cultural-phenomenons.fandom.com/wiki/Danger,_Will_Robinson){ target="blank" }
Failure to update the index to the correct setting will cause no devices to be available in Splunk Enterprise Security.
!!!

The index definition is set by a search macro. 

Macro | Default | Description
----- | ------- | -----------
`sa_#TODO_index` | index=#TODO | Index definition for #TODO asset index.

> Update the index definition to the correct index that contains the `#TODO:insightvm:asset` sourcetype.

## How to update

==- :icon-star-fill: Use Enterprise Security's Settings <small>(Recommended)</small>
1. <small>(In Splunk Enterprise Security)</small> Navigate to Configure > General > General Settings.
2. From the "App" dropdown select `SA-#TODO`.
3. Update the SA-#TODO Index definition and click "Save."
==- Update Search Macro Manually
1. Navigate to Settings > Advanced Search > Search Macros.
2. From the "App" dropdown choose `SA-#TODO`.
3. Set the "Owner" dropdown to `any`.
4. Click the macro named `sa_#TODO_index` to update the index definition.
===