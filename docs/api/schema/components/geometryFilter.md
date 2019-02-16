# Geometry Filter Schema

Filter that returns results whose bounding geometry contains the specified geographical coordinate.


| Name | Type | Accepted Values | Default |
|------|------|--------|---------|
| type **(required)**| enum| `geometry`|  |
| geometry **(required)**| oneOf| [Geometry](geo.md)|  |
  | geometry.0 **(required)**| object| |  |
  | geometry.0.type **(required)**| enum| `Point`|  |
  | geometry.0.coordinates **(required)**| array| |  |
  | geometry.1 **(required)**| | |  |
  | geometry.1.type **(required)**| enum| `MultiPoint`|  |
  | geometry.1.coordinates **(required)**| array(array)| |  |
  | geometry.2 **(required)**| | |  |
  | geometry.2.type **(required)**| enum| `LineString`|  |
  | geometry.2.coordinates **(required)**| | |  |
  | geometry.3 **(required)**| | |  |
  | geometry.3.type **(required)**| enum| `MultiLineString`|  |
  | geometry.3.coordinates **(required)**| array| |  |
  | geometry.4 **(required)**| | |  |
  | geometry.4.type **(required)**| enum| `Polygon`|  |
  | geometry.4.coordinates **(required)**| array| |  |
  | geometry.5 **(required)**| | |  |
  | geometry.5.type **(required)**| enum| `MultiPolygon`|  |
  | geometry.5.coordinates **(required)**| array(array)| |  |
| relation| enum| `contains`, `disjoint`, `intersects`, `within`| intersects |


## type **(required)**

Filter type.

### Values

#### Type:
enum


#### Accepted Values:
* geometry





## geometry **(required)**

One geometry as defined by GeoJSON

### Values

#### Type:
oneOf


#### Accepted Values:
* [Geometry](geo.md)





## relation

How the result geometry relates to the query geometry, e.g., return all datasets whose geometry contains the given point.

### Values

#### Type:
enum
#### Default:
intersects


#### Accepted Values:
* contains
* disjoint
* intersects
* within






