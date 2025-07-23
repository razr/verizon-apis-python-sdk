
# Device Role

The access rule (DeviceRole object) defines this topics the application or device can publish or subscribe to. It also defines how many parallel subscriptions one device or applications can have and how fast it can publish messages.

## Structure

`DeviceRole`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `str` | Required | The unique name of the access rule.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1000`, *Pattern*: `^[a-zA-Z0-9_$\{\}:.-]+$` |
| `subscribe_limit` | `int` | Optional | The maximum number of subscriptions that one application or device can make.<br><br>**Default**: `50`<br><br>**Constraints**: `>= 0`, `<= 2147483647` |
| `publish_rate_limit` | `int` | Optional | The maximum rate that one application or device can publish messages per seconds.<br><br>**Default**: `15`<br><br>**Constraints**: `>= 0`, `<= 2147483647` |
| `publish` | `List[str]` | Optional | The topics or topic patterns that the application or device is allowed to publish messages.<br><br>**Constraints**: *Minimum Items*: `0`, *Maximum Items*: `1000`, *Minimum Length*: `1`, *Maximum Length*: `1000`, *Pattern*: `^[a-zA-Z0-9_$\{\}*/^\|.-]+$` |
| `subscribe` | `List[str]` | Optional | The topics or topic patterns that the application or device is allowed to subscribe to.<br><br>**Constraints**: *Minimum Items*: `0`, *Maximum Items*: `1000`, *Minimum Length*: `1`, *Maximum Length*: `1000`, *Pattern*: `^[a-zA-Z0-9_$\{\}*/^\|.-]+$` |

## Example (as JSON)

```json
{
  "name": "ts.device.mqtt.imp:Software.Application.TestVendor",
  "subscribeLimit": 50,
  "publishRateLimit": 15,
  "publish": [
    "publish9",
    "publish0"
  ],
  "subscribe": [
    "subscribe7",
    "subscribe6"
  ]
}
```

