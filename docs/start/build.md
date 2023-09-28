---
order: -4
icon: workflow
label: Force build
---

# Force initial build

!!!info Optional
!!!

The initial build will not occur until the first scheduled runtime (see [Update default saved search schedule](scheduled-search.md)). To force the initial build perform the following:

1. Navigate to Settings > Searches, reports, and alerts.
2. Set the "App" dropdown to `SA-#TODO`.
3. Set the "Owner" dropdown to `All`.
4. Click "Run" under actions for the search `#TODO Assets - Lookup Gen`.

!!!info Note
The search will run in a new tab over the default time period of 60 minutes. Expand to longer timeframe for the initial build (i.e. Last 30 days). The default search is configured to run hourly to continually append new devices reported from #TODO.
!!!