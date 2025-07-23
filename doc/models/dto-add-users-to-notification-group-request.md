
# Dto Add Users to Notification Group Request

## Structure

`DtoAddUsersToNotificationGroupRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountname` | `str` | Optional | The numeric account name, which must include leading zeros |
| `id` | `str` | Optional | UUID of the user record, assigned at creation |
| `userids` | `List[str]` | Optional | - |

## Example (as JSON)

```json
{
  "accountname": "0000123456-00001",
  "id": "id4",
  "userids": [
    "userids2",
    "userids1"
  ]
}
```

