
# Rbs High Precision Tilt Config

## Structure

`RbsHighPrecisionTiltConfig`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mode` | [`ModeEnum`](../../doc/models/mode-enum.md) | Optional | the reporting mode of the tilt sensor |
| `periodic_reporting` | [`PeriodicReporting`](../../doc/models/periodic-reporting.md) | Optional | The units and values of the time interval for the sensor to send a report |
| `hold_time` | `int` | Optional | The time the threshold condition exists, in milliseconds, to recognize an event |
| `angle_away` | `int` | Optional | the threshold value, from verticle, to recognize an event |
| `angle_toward` | `int` | Optional | the threshold value, moving towards  verticle, to recognize an event |
| `tscore` | [`Tscore`](../../doc/models/tscore.md) | Optional | - |

## Example (as JSON)

```json
{
  "hold-time": 5000,
  "angle-away": 5,
  "angle-toward": 5,
  "mode": "reportOnChange",
  "periodic-reporting": {
    "unit": "minutes",
    "hours": 250,
    "minutes": 232
  }
}
```

