# Update Price Plan Triggers

```python
update_price_plan_triggers_controller = client.update_price_plan_triggers
```

## Class Name

`UpdatePricePlanTriggersController`


# Update Trigger Rules

Updates a usage trigger at the account level, device level or a price plan trigger for all devices on the account

```python
def update_trigger_rules(self,
                        body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V2TriggersRequest1`](../../doc/models/v2-triggers-request-1.md) | Body, Required | Update a trigger |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `body` property of this instance returns the response data which is of type [`TriggerResponse`](../../doc/models/trigger-response.md).

## Example Usage

```python
body = V2TriggersRequest1(
    trigger_id='b9cc1da6-ffff-eeee-gggg-7eba8859ab5e',
    trigger_name='name of the trigger',
    ecpd_id='Verizon profile ID',
    trigger_category=TriggerCategoryEnum.ACCOUNTUSAGE,
    data_trigger=DataTrigger5(),
    notification=Notificationarray(
        notification_type='PerEvent',
        callback=True,
        email_notification=False,
        notification_group_name='NotificationGroupName',
        notification_frequency_factor=3,
        notification_frequency_interval='Daily',
        external_email_recipients='ExternalEmailRecipients',
        sms_notification=True,
        sms_numbers=[
            Cellphonenumber(
                number='10-digit mobile number',
                carrier='mobile service provider'
            ),
            Cellphonenumber(
                number='10-digit mobile number',
                carrier='mobile service provider'
            )
        ],
        reminder=True,
        severity='Notice'
    ),
    active=ActiveEnum.TRUE
)

result = update_price_plan_triggers_controller.update_trigger_rules(body)

if result.is_success():
    print(result.body)
elif result.is_error():
    print(result.errors)
```

## Example Response *(as JSON)*

```json
{
  "triggerId": "be1b5958-ffff-eeee-gggg-b1b7618c0035"
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Error response | [`RuleRestErrorResponseException`](../../doc/models/rule-rest-error-response-exception.md) |

