
# Geometry Schema

Schemas for GeoJson

# Geometry Definitions

| Property | Type | Group |
|----------|------|-------|
| [coordinates](#coordinates) | [polygon](geo.md#/definitions/polygon) | `#/definitions/MultiPolygon` |
| [type](#type) | `enum` | `#/definitions/MultiPolygon` |

## coordinates


`coordinates`

* is optional
* type: [polygon](geo.md#/definitions/polygon)
* defined in this schema

### coordinates Type


Array type: [polygon](geo.md#/definitions/polygon)

All items must be of the type:

* [polygon](geo.md#/definitions/polygon)








## type


`type`

* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `MultiPolygon` |  |



