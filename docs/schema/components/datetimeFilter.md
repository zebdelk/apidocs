
#  Schema

```
```


| Abstract | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|--------------|-------------------|-----------------------|------------|
| Can be instantiated | No | Experimental | No | Forbidden | Forbidden | [schema/components/datetimeFilter.json](schema/components/datetimeFilter.json) |

#  Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [after](#after) | `string` | Optional |  (this schema) |
| [before](#before) | `string` | Optional |  (this schema) |
| [relation](#relation) | `enum` | Optional |  (this schema) |
| [type](#type) | `enum` | **Required** |  (this schema) |

## after


`after`

* is optional
* type: `string`
* defined in this schema

### after Type


`string`

* format: `date-time` – date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))






## before


`before`

* is optional
* type: `string`
* defined in this schema

### before Type


`string`

* format: `date-time` – date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))






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
| `datetime` |  |



