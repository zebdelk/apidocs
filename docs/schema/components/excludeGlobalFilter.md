
#  Schema

```
```

Flag to request that geospatially global results be excluded. Defaults to false if not provided.

| Abstract | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|--------------|-------------------|-----------------------|------------|
| Can be instantiated | No | Experimental | No | Forbidden | Forbidden | [schema/components/excludeGlobalFilter.json](schema/components/excludeGlobalFilter.json) |

#  Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [type](#type) | `enum` | **Required** |  (this schema) |
| [value](#value) | `boolean` | **Required** |  (this schema) |

## type


`type`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `excludeGlobal` |  |




## value


`value`

* is **required**
* type: `boolean`
* defined in this schema

### value Type


`boolean`




