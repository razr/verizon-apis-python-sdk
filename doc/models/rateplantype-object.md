
# Rateplantype Object

## Structure

`RateplantypeObject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `rate_plan_group_description` | `str` | Optional | - |
| `rate_plan_type` | `str` | Optional | - |
| `rate_plan` | [`List[Rateplantype2]`](../../doc/models/rateplantype-2.md) | Optional | An array of rateplan names |

## Example (as JSON)

```json
{
  "ratePlanGroupDescription": "AGS Description_73",
  "ratePlanType": "ratePlanType2",
  "ratePlan": [
    {
      "description": "description2",
      "sizeKb": "sizeKb2",
      "carrierRatePlanCode": "carrierRatePlanCode8",
      "zeroDollarBilling": false,
      "promotionOffered": false
    },
    {
      "description": "description2",
      "sizeKb": "sizeKb2",
      "carrierRatePlanCode": "carrierRatePlanCode8",
      "zeroDollarBilling": false,
      "promotionOffered": false
    }
  ]
}
```

