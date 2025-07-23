
# Dto Sensor Off Board Status Request

## Structure

`DtoSensorOffBoardStatusRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountname` | `str` | Optional | The numeric account name, which must include leading zeros |
| `gatewayidentifier` | [`Gatewayidentifier`](../../doc/models/gatewayidentifier.md) | Optional | - |
| `offboarding` | [`Offboarding`](../../doc/models/offboarding.md) | Optional | - |

## Example (as JSON)

```json
{
  "accountname": "0000123456-00001",
  "gatewayidentifier": {
    "deviceid": "deviceid0"
  },
  "offboarding": {
    "sensoridentifier": "sensoridentifier8"
  }
}
```

