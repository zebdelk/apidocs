
# Collection Filter Schema

Collections to filter results by (logical OR if multiple filters or multiple values in one filter). If any collection filters are provided, granules are returned.

# Collection Filter Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [type](#type) | `enum` | **Required** | Collection Filter (this schema) |
| [values](#values) | `array`: `string[]` | **Required** | Collection Filter (this schema) |

## type


`type`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `collection` |  |




## values


`values`

* is **required**
* type: `array`: `string[]`
* defined in this schema

### values Type


Array type: `array`: `string[]`

All items must be of the type:
`string`








