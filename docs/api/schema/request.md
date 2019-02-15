
# Search Request Schema

The shape of a search request body that can be sent to the OneStop API to execute a search against available metadata. Collections are returned by default unless a collection filter is included, resulting in granules being returned.

# Search Request Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [facets](#facets) | `boolean` | Optional | Search Request (this schema) |
| [filters](#filters) | [filter](components/filter.md) | Optional | Search Request (this schema) |
| [page](#page) | `object` | Optional | Search Request (this schema) |
| [queries](#queries) | [query](components/query.md) | Optional | Search Request (this schema) |
| [summary](#summary) | `boolean` | Optional | Search Request (this schema) |

## facets

Flag to request counts of results by GCMD keywords in addition to results. Defaults to false if not provided.

`facets`

* is optional
* type: `boolean`
* defined in this schema

### facets Type


`boolean`





## filters


`filters`

* is optional
* type: [filter](components/filter.md)
* defined in this schema

### filters Type


Array type: [filter](components/filter.md)

All items must be of the type:

* [filter](components/filter.md)








## page

Pagination of results

`page`

* is optional
* type: `object`
* defined in this schema

### page Type


`object` with following properties:


| Property | Type | Required |
|----------|------|----------|
| `max`| integer | **Required** |
| `offset`| integer | **Required** |



#### max

Maximum number of results returned. If the page object is not provided, this defaults to 10.

`max`

* is **required**
* type: `integer`

##### max Type


`integer`

* minimum value: `0`
* maximum value: `1000`







#### offset

Number of records by which to offset results. If the page object is not provided, this defaults to 0.

`offset`

* is **required**
* type: `integer`

##### offset Type


`integer`












## queries


`queries`

* is optional
* type: [query](components/query.md)
* defined in this schema

### queries Type


Array type: [query](components/query.md)

All items must be of the type:

* [query](components/query.md)








## summary

Flag to request summary of search results instead of full set of attributes. Defaults to true if not provided.

`summary`

* is optional
* type: `boolean`
* defined in this schema

### summary Type


`boolean`




