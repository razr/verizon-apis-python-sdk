
# Actionobject

## Structure

`Actionobject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `suspend` | `bool` | Optional | - |
| `suspend_details` | [`Suspenddetailsobject`](../../doc/models/suspenddetailsobject.md) | Optional | - |
| `change_plan` | `bool` | Optional | a flag to set if the trigger changes service plans, true, or not, false |
| `change_plan_details` | [`ChangePlanDetails`](../../doc/models/change-plan-details.md) | Optional | The service plan code to switch to |

## Example (as JSON)

```json
{
  "suspend": true,
  "changePlan": true,
  "suspendDetails": {
    "suspendFromAccounts": [
      "suspendFromAccounts7"
    ],
    "suspendDuration": 152,
    "suspendOption": "suspendOption2",
    "threshold": 166,
    "thresholdUnit": "GB"
  },
  "changePlanDetails": {
    "toCarrierServicePlanCode": "toCarrierServicePlanCode2"
  }
}
```

