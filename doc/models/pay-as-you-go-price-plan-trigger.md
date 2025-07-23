
# Pay as You Go Price Plan Trigger

## Structure

`PayAsYouGoPricePlanTrigger`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `pay_as_you_go` | [`PayAsYouGoFilterCriteria`](../../doc/models/pay-as-you-go-filter-criteria.md) | Optional | - |
| `condition` | [`Rateplantype2Condition`](../../doc/models/rateplantype-2-condition.md) | Optional | - |
| `action` | [`Actionobject`](../../doc/models/actionobject.md) | Optional | - |

## Example (as JSON)

```json
{
  "payAsYouGo": {
    "filterCriteria": {
      "carrierServicePlanCode": "carrierServicePlanCode4",
      "accountNameList": [
        "accountNameList7",
        "accountNameList8"
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
  "action": {
    "suspend": false,
    "suspendDetails": {
      "suspendFromAccounts": [
        "suspendFromAccounts7"
      ],
      "suspendDuration": 152,
      "suspendOption": "suspendOption2",
      "threshold": 166,
      "thresholdUnit": "GB"
    },
    "changePlan": false,
    "changePlanDetails": {
      "toCarrierServicePlanCode": "toCarrierServicePlanCode2"
    }
  }
}
```

