
# Geometry Filter Schema

Filter that returns results whose bounding geometry contains the specified geographical coordinate.

# Geometry Filter Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [geometry](#geometry) | [Geometry](geo.md#/Geometry) | **Required** | Geometry Filter (this schema) |
| [relation](#relation) | `enum` | Optional | Geometry Filter (this schema) |
| [type](#type) | `enum` | **Required** | Geometry Filter (this schema) |

## geometry


`geometry`

* is **required**
* type: [Geometry](geo.md#/Geometry)
* defined in this schema

### geometry Type



* [Geometry](geo.md#/Geometry)





## relation

How the result geometry relates to the query geometry, e.g., return all datasets whose geometry contains the given point. Defaults to 'intersects'.

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
| `geometry` |  |


