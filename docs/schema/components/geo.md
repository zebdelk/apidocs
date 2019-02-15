
#  Schema

```
```


| Abstract | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|--------------|-------------------|-----------------------|------------|
| Cannot be instantiated | Yes | Experimental | No | Forbidden | Permitted | [schema/components/geo.json](schema/components/geo.json) |

#  Definitions

| Property | Type | Group |
|----------|------|-------|
| [coordinates](#coordinates) | reference | `#/definitions/MultiPolygon` |
| [type](#type) | `enum` | `#/definitions/MultiPolygon` |

## coordinates


`coordinates`

* is optional
* type: reference
* defined in this schema

### coordinates Type


Array type: reference

All items must be of the type:

* [polygon](schema/components/geo.md#/definitions/polygon)








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



