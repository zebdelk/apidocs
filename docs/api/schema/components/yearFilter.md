
# Year Filter Schema

Filter results by before, after, or a date range. Differs from the Datetime Filter in that it handles year values only.

# Year Filter Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [after](#after) | `number` | Optional | Year Filter (this schema) |
| [before](#before) | `number` | Optional | Year Filter (this schema) |
| [relation](#relation) | `enum` | Optional | Year Filter (this schema) |
| [type](#type) | `enum` | **Required** | Year Filter (this schema) |

## after


`after`

* is optional
* type: `number`
* defined in this schema

### after Type


`number`


* must be a multiple of `1`





## before


`before`

* is optional
* type: `number`
* defined in this schema

### before Type


`number`


* must be a multiple of `1`





## relation

How the result time range relates to the query time range, e.g., return all datasets whose time range is within the given time range. Defaults to 'intersects'.

`relation`

* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#relation-known-values).

### relation Known Values
| Value | Description |
|-------|-------------|
| `contains` |  |
| `disjoint` |  |
| `intersects` |  |
| `within` |  |




## type


`type`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `year` |  |



