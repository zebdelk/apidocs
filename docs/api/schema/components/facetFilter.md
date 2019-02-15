
# Facet Filter Schema

```
```

Filters results based on given GCMD keywords where returned results MUST have the specified keyword. Multiple facetFilter objects will be combined with logical AND; multiple values in a single facetFilter object will be combined with the logical OR.

# Facet Filter Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [name](#name) | `enum` | **Required** | Facet Filter (this schema) |
| [type](#type) | `enum` | **Required** | Facet Filter (this schema) |
| [values](#values) | `string[]` | **Required** | Facet Filter (this schema) |

## name

One of the GCMD keyword categories: science, services, locations, instruments, platforms, projects, dataCenters, horizontalResolution, verticalResolution, temporalResolution.

`name`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#name-known-values).

### name Known Values
| Value | Description |
|-------|-------------|
| `science` |  |
| `services` |  |
| `locations` |  |
| `instruments` |  |
| `platforms` |  |
| `projects` |  |
| `dataCenters` |  |
| `horizontalResolution` |  |
| `verticalResolution` |  |
| `temporalResolution` |  |




## type


`type`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `facet` |  |




## values

Exact match GCMD keyword(s), e.g., "Atmosphere > Atmospheric Temperature > Surface Temperature"

`values`

* is **required**
* type: `string[]`
* defined in this schema

### values Type


Array type: `string[]`

All items must be of the type:
`string`









