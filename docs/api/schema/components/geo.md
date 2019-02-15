
# Geometry Schema

Schemas for GeoJson

# Geometry Definitions

| Property | Type | Group |
|----------|------|-------|
| [coordinates](#coordinates) | `array`: [polygon](geo.md#/definitions/polygon) | `#/definitions/MultiPolygon` |
| [type](#type) | `enum` | `#/definitions/MultiPolygon` |

## coordinates


`coordinates`

* is optional
* type: `array`: [polygon](geo.md#/definitions/polygon)


### coordinates Type


Array type: `array`: [polygon](geo.md#/definitions/polygon)

All items must be of the type:

* [polygon](geo.md#/definitions/polygon)







## type


`type`

* is optional
* type: `enum`

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `MultiPolygon` |  |



