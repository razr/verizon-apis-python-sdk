
# Account Level Filter

## Structure

`AccountLevelFilter`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `separate_or_combined` | `str` | Optional | Determines whether or not to aggregate usage of multiple accounts together, or separate by account. If this is null or not present, then the trigger will be for an individual line. |
| `account_names` | [`Accountnames`](../../doc/models/accountnames.md) | Optional | - |

## Example (as JSON)

```json
{
  "separateOrCombined": "Separate",
  "accountNames": {
    "accountNameList": [
      "accountNameList7",
      "accountNameList8",
      "accountNameList9"
    ]
  }
}
```

