
# App Config Response Error Exception

error response structure

## Structure

`AppConfigResponseErrorException`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `error` | `str` | Required | The short summary of the error<br><br>**Constraints**: *Minimum Length*: `0`, *Maximum Length*: `1024`, *Pattern*: ``^[\w~\+\-!@#$%^&*()\`\[\]{=};\"':,.\\\/<>?\|\s]*$`` |
| `description` | `str` | Required | The detailed description of the error<br><br>**Constraints**: *Minimum Length*: `0`, *Maximum Length*: `8192`, *Pattern*: ``^[\w~\+\-!@#$%^&*()\`\[\]{=};\"':,.\\\/<>?\|\s]*$`` |

## Example (as JSON)

```json
{
  "error": "Error Summary",
  "description": "Error Description"
}
```

