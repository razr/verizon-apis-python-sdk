
# Account Share Price Plan Trigger

## Structure

`AccountSharePricePlanTrigger`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `account_share` | [`AccountShareFilterCriteria`](../../doc/models/account-share-filter-criteria.md) | Optional | - |
| `condition` | [`Rateplantype2Condition`](../../doc/models/rateplantype-2-condition.md) | Optional | - |
| `change_plan` | `bool` | Optional | a flag to set if the trigger changes service plans, true, or not, false |
| `change_plan_details` | [`ChangePlanDetails`](../../doc/models/change-plan-details.md) | Optional | The service plan code to switch to |

## Example (as JSON)

```json
{
  "changePlan": true,
  "accountShare": {
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
  "changePlanDetails": {
    "toCarrierServicePlanCode": "toCarrierServicePlanCode2"
  }
}
```

