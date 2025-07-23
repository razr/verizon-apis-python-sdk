
# Price Plan Trigger 1

## Structure

`PricePlanTrigger1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `account_group_share` | [`AccountGroupShareIndividual1`](../../doc/models/account-group-share-individual-1.md) | Optional | - |
| `account_share` | [`AccountShareFilterCriteria`](../../doc/models/account-share-filter-criteria.md) | Optional | - |
| `condition` | [`Rateplantype2Condition`](../../doc/models/rateplantype-2-condition.md) | Optional | - |
| `change_plan` | `bool` | Optional | a flag to set if the trigger changes service plans, true, or not, false |
| `change_plan_details` | [`ChangePlanDetails`](../../doc/models/change-plan-details.md) | Optional | The service plan code to switch to |
| `pay_as_you_go` | [`PayAsYouGoFilterCriteria`](../../doc/models/pay-as-you-go-filter-criteria.md) | Optional | - |
| `action` | [`Actionobject`](../../doc/models/actionobject.md) | Optional | - |
| `stand_alone` | [`FiltercriteriaObjectCall`](../../doc/models/filtercriteria-object-call.md) | Optional | - |

## Example (as JSON)

```json
{
  "changePlan": true,
  "accountGroupShare": {
    "accountGroupShareIndividual": {
      "filterCriteria": {
        "ratePlanGroupId": 202
      },
      "condition": {
        "action": "notify"
      },
      "action": {
        "notify": {
          "alertType": "alertType8",
          "threshold": [
            {
              "carrierCode": "carrierCode4",
              "percentage": {
                "percentage50": false,
                "percentage75": false,
                "percentage90": false,
                "percentage100": false
              }
            },
            {
              "carrierCode": "carrierCode4",
              "percentage": {
                "percentage50": false,
                "percentage75": false,
                "percentage90": false,
                "percentage100": false
              }
            },
            {
              "carrierCode": "carrierCode4",
              "percentage": {
                "percentage50": false,
                "percentage75": false,
                "percentage90": false,
                "percentage100": false
              }
            }
          ]
        }
      }
    }
  },
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

