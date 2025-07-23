
# Account Level Object

## Structure

`AccountLevelObject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `filter_criteria` | [`AccountLevelFilter`](../../doc/models/account-level-filter.md) | Optional | - |
| `condition` | [`Rateplantype2Condition`](../../doc/models/rateplantype-2-condition.md) | Optional | - |
| `action` | [`AccountLevelActionEnum`](../../doc/models/account-level-action-enum.md) | Optional | The action taken when trigger conditions are met |

## Example (as JSON)

```json
{
  "action": "notify",
  "filterCriteria": {
    "separateOrCombined": "separateOrCombined4",
    "accountNames": {
      "accountNameList": [
        "accountNameList7",
        "accountNameList8",
        "accountNameList9"
      ]
    }
  },
  "condition": {
    "conditionType": "Aging",
    "comparitor": "eq",
    "threshold": 98,
    "thresholdUnit": "MB",
    "cycleType": "Weekly"
  }
}
```

