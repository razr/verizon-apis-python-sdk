
# Connection Response V3

response for api/v3/clients/connection

## Structure

`ConnectionResponseV3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mqtt_ur_ls` | `List[str]` | Required | **Constraints**: *Minimum Items*: `1`, *Maximum Items*: `20`, *Maximum Length*: `1024`, *Pattern*: `^(http?mqtt)://[^\s/$.?#].[^\s]*$` |

## Example (as JSON)

```json
{
  "MqttURLs": [
    "MqttURLs4",
    "MqttURLs5",
    "MqttURLs6"
  ]
}
```

