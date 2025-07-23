
# Data Trigger

## Structure

`DataTrigger`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `account_level` | [`AccountLevelObject`](../../doc/models/account-level-object.md) | Optional | - |

## Example (as JSON)

```json
{
  "accountLevel": {
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
    },
    "action": "suspend"
  }
}
```

