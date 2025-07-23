
# Multi Line String

A MultiLineString is a type of geometry that represents a collection of LineString geometries.

## Structure

`MultiLineString`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`MultiLineStringTypeEnum`](../../doc/models/multi-line-string-type-enum.md) | Required | - |
| `coordinates` | `List[float]` | Required | **Constraints**: *Minimum Items*: `1`, *Maximum Items*: `10`, `>= -180`, `<= 180` |

## Example (as JSON)

```json
{
  "type": "MultiLineString",
  "coordinates": [
    [
      [
        180.0,
        180.0
      ],
      [
        180.0,
        180.0
      ]
    ],
    [
      [
        180.0,
        180.0
      ],
      [
        180.0,
        180.0
      ]
    ]
  ]
}
```

