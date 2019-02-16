

# Geometry Filter Schema

Filter that returns results whose bounding geometry contains the specified geographical coordinate.


| Name | Type | Accepted Values | Default |
|------|------|--------|---------|
| type **(required)**| | `geometry`|  |
| geometry **(required)**| oneOf| |  |
| relation| | `contains`, `disjoint`, `intersects`, `within`| intersects |


## type **(required)**

Filter type.

### Values

#### Type:


#### Accepted Values:
`geometry`

## geometry **(required)**

One geometry as defined by GeoJSON

### Values

#### Type:
oneOf

#### Accepted Values:


## relation

How the result geometry relates to the query geometry, e.g., return all datasets whose geometry contains the given point.

### Values

#### Type:

#### Default:
intersects

#### Accepted Values:
`contains`, `disjoint`, `intersects`, `within`


