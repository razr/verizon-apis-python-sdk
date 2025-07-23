
# Multi Polygon

A MultiPolygon is a type of geometry that represents a collection of Polygon geometries.

## Structure

`MultiPolygon`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`MultiPolygonTypeEnum`](../../doc/models/multi-polygon-type-enum.md) | Required | - |
| `coordinates` | `List[float]` | Required | **Constraints**: *Minimum Items*: `1`, *Maximum Items*: `10`, `>= -180`, `<= 180` |

## Example (as JSON)

```json
{
  "type": "MultiPolygon",
  "coordinates": [
    [
      [
        [
          46.55
        ]
      ]
    ]
  ]
}
```

