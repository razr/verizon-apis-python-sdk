
# Data Trigger 2

## Structure

`DataTrigger2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `device_group` | [`DeviceGroupFilterCriteria`](../../doc/models/device-group-filter-criteria.md) | Optional | - |
| `condition_type` | [`ConditionTypeEnum`](../../doc/models/condition-type-enum.md) | Optional | The condition type being monitored |
| `comparitor` | [`ComparitorEnum`](../../doc/models/comparitor-enum.md) | Optional | The boolean of the comparison. `gt` is Greater Than, `lt` is Less Than and `eq` is Equal To |
| `threshold` | `int` | Optional | The threshold value the trigger monitors for |
| `threshold_unit` | [`ThresholdUnitEnum`](../../doc/models/threshold-unit-enum.md) | Optional | The units of the threshold. This can be KB, Kilobits, MB, Megabits, or GB, Gigabits |
| `cycle_type` | [`RulesCycleTypeEnum`](../../doc/models/rules-cycle-type-enum.md) | Optional | The interval to monitor for the threshold. This can be Daily, Weekly or Monthly |
| `allowance_threshold` | [`AllowanceThreshold`](../../doc/models/allowance-threshold.md) | Optional | - |
| `action` | [`Actionobject`](../../doc/models/actionobject.md) | Optional | - |

## Example (as JSON)

```json
{
  "conditionType": "Aging",
  "comparitor": "gt",
  "threshold": 100,
  "thresholdUnit": "KB",
  "cycleType": "Daily",
  "deviceGroup": {
    "filterCriteria": {
      "deviceGroupName": "deviceGroupName4",
      "IndividualOrCombined": "IndividualOrCombined4",
      "accountName": "accountName0"
    }
  }
}
```

