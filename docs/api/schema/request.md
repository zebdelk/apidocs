
# Search Request Schema

The shape of a search request body that can be sent to the OneStop API to execute a search against available metadata. Collections are returned by default unless a collection filter is included, resulting in granules being returned.

# Search Request Properties

| Property | Type | Required |
|----------|------|----------|
| [facets](#facets) | `boolean` | Optional |
| [filters](#filters) | `array`: [filter](components/filter.md) | Optional |
| [page](#page) | `object` | Optional |
| [queries](#queries) | `array`: [query](components/query.md) | Optional |
| [summary](#summary) | `boolean` | Optional |

## facets

Flag to request counts of results by GCMD keywords in addition to results. Defaults to false if not provided.

`facets`

* is optional
* type: `boolean`

### facets Type


`boolean`




## filters


`filters`

* is optional
* type: `array`: [filter](components/filter.md)


### filters Type


Array type: `array`: [filter](components/filter.md)

All items must be of the type:

* [filter](components/filter.md)







## page

Pagination of results

`page`

* is optional
* type: `object`

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
* type: `array`: [query](components/query.md)


### queries Type


Array type: `array`: [query](components/query.md)

All items must be of the type:

* [query](components/query.md)







## summary

Flag to request summary of search results instead of full set of attributes. Defaults to true if not provided.

`summary`

* is optional
* type: `boolean`

### summary Type


`boolean`



