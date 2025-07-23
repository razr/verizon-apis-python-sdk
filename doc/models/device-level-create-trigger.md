
# Device Level Create Trigger

## Structure

`DeviceLevelCreateTrigger`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `trigger_name` | `str` | Optional | The user defined name of the trigger |
| `ecpd_id` | `str` | Optional | The Enterprise Customer Profile Database ID |
| `trigger_category` | [`TriggerCategoryEnum`](../../doc/models/trigger-category-enum.md) | Optional | The type of trigger being created or modified |
| `data_trigger` | [`DataTrigger2`](../../doc/models/data-trigger-2.md) | Optional | - |
| `notification` | [`Notificationarray`](../../doc/models/notificationarray.md) | Optional | - |

## Example (as JSON)

```json
{
  "triggerName": "name of the trigger",
  "ecpdId": "Verizon profile ID",
  "triggerCategory": "PricePlanDataUsage",
  "dataTrigger": {
    "deviceGroup": {
      "filterCriteria": {
        "deviceGroupName": "deviceGroupName4",
        "IndividualOrCombined": "IndividualOrCombined4",
        "accountName": "accountName0"
      }
    },
    "conditionType": "Aging",
    "comparitor": "eq",
    "threshold": 222,
    "thresholdUnit": "MB"
  },
  "notification": {
    "notificationType": "notificationType8",
    "callback": false,
    "emailNotification": false,
    "notificationGroupName": "notificationGroupName6",
    "notificationFrequencyFactor": 22
  }
}
```

