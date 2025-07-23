
# Pay as You Go Update Trigger Request

## Structure

`PayAsYouGoUpdateTriggerRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `trigger_id` | `str` | Optional | The system assigned UUID of the trigger |
| `trigger_name` | `str` | Optional | The user defined name of the trigger |
| `ecpd_id` | `str` | Optional | The Enterprise Customer Profile Database ID |
| `trigger_category` | [`TriggerCategoryEnum`](../../doc/models/trigger-category-enum.md) | Optional | The type of trigger being created or modified |
| `price_plan_trigger` | [`PayAsYouGoPricePlanTrigger`](../../doc/models/pay-as-you-go-price-plan-trigger.md) | Optional | - |
| `notification` | [`Notificationarray`](../../doc/models/notificationarray.md) | Optional | - |
| `active` | [`ActiveEnum`](../../doc/models/active-enum.md) | Optional | A flag to indicate of the trigger is active, true, or not, false |

## Example (as JSON)

```json
{
  "triggerId": "be1b5958-ffff-eeee-gggg-b1b7618c0035",
  "triggerName": "name of the trigger",
  "ecpdId": "Verizon profile ID",
  "active": "true",
  "triggerCategory": "PricePlanDataUsage",
  "pricePlanTrigger": {
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
}
```

