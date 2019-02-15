
# Text Query Schema

Text query to search with that is valid so long as it does not have a leading wildcard ('*' or '?')

# Text Query Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [type](#type) | `enum` | **Required** | Text Query (this schema) |
| [value](#value) | `string` | **Required** | Text Query (this schema) |

## type


`type`

* is **required**
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `queryText` |  |




## value


`value`

* is **required**
* type: `string`
* defined in this schema

### value Type


`string`



All instances must conform to this regular expression 
(test examples [here](https://regexr.com/?expression=%5E(%3F!%5Cs*%5B%5C*%5C%3F%5D%2B).*)):
```regex
^(?!\s*[\*\?]+).*
```





