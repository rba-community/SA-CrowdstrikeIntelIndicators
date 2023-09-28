# Update Cleanup

The saved search `#TODO Assets - Lookup Cleanup` runs every day at 3:03 am to remove old/stale device data from the kvstore. By default, it will remove any device that has not reported in longer than 31 days.

!!!info Note
Even though an asset may be removed, it will be re-added by the saved search `#TODO Assets - Lookup Gen` if it is found in the data again.
!!!

## Update Search Macro

To change the retention period from the default, there is a search macro that will need to be updated.

1. Navigate to Settings > Advanced Search > Search Macros.
2. Set the "App" to `SA-#TODO`.
3. Set the "Owner" to `Any`.
4. Click on `sa_#TODO_retention` to modify the definition.
5. Set the definition to a valid [time modifier<small>:icon-link-external:</small>](https://docs.splunk.com/Documentation/Splunk/latest/SearchReference/SearchTimeModifiers#How_to_specify_relative_time_modifiers){ target="blank" }.

!!!success Note
__Make sure to keep the quotes around the definition.__
i.e. "-7d\@d"
!!!

## Update Cleanup Search Schedule

It may also be necessary to update how often the cleanup search runs (default: Monthly).

To update the default schedule perform the following steps:

1. Navigate to Settings > Searches, reports, and alerts.
1. Set the "App" dropdown to `SA-#TODOAssets`.
1. Set the "Owner" dropdown to `All`.
1. Click "Edit" under actions for the search `#TODO Assets - Lookup Cleanup`
1. Click "Edit Schedule" and update the schedule and necessary.
