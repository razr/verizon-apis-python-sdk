
# Device Group Filter

## Structure

`DeviceGroupFilter`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `device_group_name` | `str` | Optional | - |
| `individual_or_combined` | `str` | Optional | - |
| `account_name` | `str` | Optional | The numeric name of the account and must include leading zeroes |

## Example (as JSON)

```json
{
  "deviceGroupName": "User defined group name",
  "IndividualOrCombined": "Combined",
  "accountName": "0000123456-00001"
}
```

