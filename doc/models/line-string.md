
# Line String

A LineString is a type of geometry that represents a collection of points that are connected by line segments.

## Structure

`LineString`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`LineStringTypeEnum`](../../doc/models/line-string-type-enum.md) | Required | - |
| `coordinates` | `List[float]` | Required | **Constraints**: *Minimum Items*: `2`, *Maximum Items*: `63`, `>= -180`, `<= 180` |

## Example (as JSON)

```json
{
  "type": "LineString",
  "coordinates": [
    [
      51.53,
      51.54
    ],
    [
      51.53,
      51.54
    ]
  ]
}
```

