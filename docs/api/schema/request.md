

# Search Request Schema

The shape of a search request body that can be sent to the OneStop API to execute a search against available metadata. Collections are returned by default unless a collection filter is included, resulting in granules being returned.


| Name | Type | Accepted Values | Default |
|------|------|--------|---------|
| queries| array| [Query](components/query.md)|  |
| filters| array| [Filter](components/filter.md)|  |
| facets| boolean| | false |
| summary| boolean| | true |
| page| object| [Pagination](components/page.md)|  |


## queries


### Values

#### Type:
array

#### Accepted Values:
[Query](components/query.md)

## filters


### Values

#### Type:
array

#### Accepted Values:
[Filter](components/filter.md)

## facets

Flag to request counts of results by GCMD keywords in addition to results.

### Values

#### Type:
boolean

#### Accepted Values:


## summary

Flag to request summary of search results instead of full set of attributes.

### Values

#### Type:
boolean
#### Default:
true

#### Accepted Values:


## page

Pagination of results

### Values

#### Type:
object

#### Accepted Values:
[Pagination](components/page.md)


