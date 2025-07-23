
# Suspenddetailsobject

## Structure

`Suspenddetailsobject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `suspend_from_accounts` | `List[str]` | Optional | - |
| `suspend_duration` | `int` | Optional | - |
| `suspend_option` | `str` | Optional | - |
| `threshold` | `int` | Optional | The threshold value the trigger monitors for |
| `threshold_unit` | [`ThresholdUnitEnum`](../../doc/models/threshold-unit-enum.md) | Optional | The units of the threshold. This can be KB, Kilobits, MB, Megabits, or GB, Gigabits |

## Example (as JSON)

```json
{
  "suspendDuration": 90,
  "suspendOption": "withBilling",
  "threshold": 100,
  "thresholdUnit": "KB",
  "suspendFromAccounts": [
    "suspendFromAccounts7",
    "suspendFromAccounts8",
    "suspendFromAccounts9"
  ]
}
```

