# All Configurations

# TODO - DELETE THIS LINE - Example Only

Below is a table that list all configuration for this add-on.

Name | Type | Web Location | CLI Location\* | Description
---- | ---- | ------------ | ------------- | -----------
#TODO Assets - Lookup Gen | Saved Search | Settings > Searches reports, and alerts | savedsearches.conf | Populates the lookup file `sa_#TODO_assets`.
#TODO Assets - Lookup Cleanup | Saved Search | Settings > Searches reports, and alerts | savedsearches.conf | removes old entries from kvstore lookup: `sa_#TODO_assets`.
sa_#TODO_assets | lookup | Settings > Lookups > Lookup definitions | transforms.conf | Lookup definition for the KVStore collection `sa_#TODO_assets_collection`.
sa_#TODO_assets_collection | KVStore collection | n/a\*\* | collections.conf | KVStore configuration.
sa_#TODO_index | Search macro | Settings > Advanced Search > Search Macros | macros.conf | Index definition for the #TODO index that contains the sourcetype `#TODO:insightvm:asset`.
sa_#TODO_retention | Search macro | Settings> Advanced Search > Search Macros | macros.conf | The amount of time for the device not being updated before it is removed from the lookup. `default "-31d"`
identity_manager://sa_#TODO_assets | Asset lookup configuration | Enterprise Security > Configure > Data Enrichment > Asset and Identity Management > Asset Lookups | inputs.conf | Asset configuration lookup to load #TODO Assets into the asset database.

> \*CLI locations are relative to `../default`. Any update to CLI configuration files should be done in the local directory.

!!!info
**If you have the [Splunk App for Lookup File Editing<small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/263){ target="blank" }, the KVStore collection `sa_#TODO_assets_collection` is viewable within the Web interface.
!!!