
# Rateplantype 2

## Structure

`Rateplantype2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `description` | `str` | Optional | - |
| `size_kb` | `str` | Optional | - |
| `carrier_rate_plan_code` | `str` | Optional | - |
| `zero_dollar_billing` | `bool` | Optional | - |
| `promotion_offered` | `bool` | Optional | - |
| `promotion_days` | `int` | Optional | - |
| `rate_plan_type` | `str` | Optional | - |
| `account` | [`List[Accountid]`](../../doc/models/accountid.md) | Optional | Account information |

## Example (as JSON)

```json
{
  "description": "PlanDescription 2",
  "sizeKb": "1048576",
  "carrierRatePlanCode": "Service plan code value",
  "zeroDollarBilling": false,
  "promotionOffered": false,
  "promotionDays": -2147483648
}
```

