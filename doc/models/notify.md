
# Notify

## Structure

`Notify`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `alert_type` | `str` | Optional | - |
| `threshold` | [`List[Carriercode1]`](../../doc/models/carriercode-1.md) | Optional | - |

## Example (as JSON)

```json
{
  "alertType": "individualpriceplan",
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
```

