# Priority Field

!!!primary To update the `priority` field modify the `#TODO Assets - Lookup Gen` saved search. It is recommended to clone the default search before making changes (see [Clone Saved Search](clone-search.md)).
!!!

The priority field is very generic by default and should be updated to suite your environment. The following table describes how this field is set.

Type | Condition | Severity | Description
---- | --------- | -------- | -----------
Expression | exploits>=1 | `critical` | Any system with more than 1 exploit is set to critical.
RegEx\* | server | `high` | Sets systems categorized as "servers" to high.
Expression | critical_vulnerabilities>=1 | `high` | Systems with more than one critical vulnerability is set to high.
Expression | risk_score>=upper_risk | `high` | Systems in the top 5% of risk are set to high.
Expression | moderate_vulnerabilities>=1 | `medium` | Systems with more than one moderate vulnerability are set to medium.
boolean | true() | `low` | catch-all. Remaining devices receive low severity.


> \*Regex Match is performed on the category field.

Default priority field definition

```python
priority=case(
    exploits>=1, "critical", 
    match(category, "(?i)server"), "high", 
    critical_vulnerabilities>=1, "high", 
    risk_score>=upper_risk, "high",
    moderate_vulnerabilities>=1, "medium", 
    true(), "low"
    )
```
