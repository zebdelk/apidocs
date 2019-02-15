
# Collection Filter Schema

Collections to filter results by (logical OR if multiple filters or multiple values in one filter). If any collection filters are provided, granules are returned.

# Collection Filter Properties

| Property | Type | Required |
|----------|------|----------|
| [type](#type) | `enum` | **Required** |
| [values](#values) | `array`: `string[]` | **Required** |

## type


`type`

* is **required**
* type: `enum`

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `collection` |  |




## values


`values`

* is **required**
* type: `array`: `string[]`


### values Type


Array type: `array`: `string[]`

All items must be of the type:
`string`








