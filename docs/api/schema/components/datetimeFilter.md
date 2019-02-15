
# Datetime Filter Schema

Filter results by before, after, or a date range.

# Datetime Filter Properties

| Property | Type | Required |
|----------|------|----------|
| [after](#after) | `string` | Optional |
| [before](#before) | `string` | Optional |
| [relation](#relation) | `enum` | Optional |
| [type](#type) | `enum` | **Required** |

## after


`after`

* is optional
* type: `string`

### after Type


`string`

* format: `date-time` – date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))





## before


`before`

* is optional
* type: `string`

### before Type


`string`

* format: `date-time` – date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))





## relation

How the result time range relates to the query time range, e.g., return all datasets whose time range is within the given time range. Defaults to 'intersects'.

`relation`

* is optional
* type: `enum`

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

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `datetime` |  |



