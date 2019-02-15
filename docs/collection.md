# Collection API



## Table of Contents

* [Paths](#paths)
  - [`HEAD` /collection](#op-head-collection) 
  - [`GET` /collection](#op-get-collection) 
  - [`HEAD` /collection/{id}](#op-head-collection-id) 
  - [`GET` /collection/{id}](#op-get-collection-id) 
  - [`POST` /search/collection](#op-post-search-collection) 




## Paths

### <span id="op-head-collection" > `HEAD` /collection </span>
> Get Collection Info








#### Responses



##### ▶ 200 - Successful operation

###### Headers
_No headers specified_


#### Tags

<div class="tags">
  <div class="tags__tag"></div>
</div>
</div>

### `GET` /collection #{op-get-collection}
> Get Collection Info








#### Responses



##### ▶ 200 - Successful operation

###### Headers
_No headers specified_

###### application/json


[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>data</td>
        <td>
          array(object)
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>data.type</td>
        <td>
          string
        </td>
        <td></td>
        <td><code>count</code></td>
      </tr>
      <tr>
        <td>data.id</td>
        <td>
          string
        </td>
        <td></td>
        <td><code>collection</code>, <code>granule</code></td>
      </tr>
      <tr>
        <td>data.count</td>
        <td>
          integer
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>


##### Example _(generated)_

```json
{
  "data": [
    {
      "type": "count",
      "id": "collection",
      "count": 0
    }
  ]
}
```

#### Tags

<div class="tags">
  <div class="tags__tag"></div>
</div>
</div>

### `HEAD` /collection/{id} #{op-head-collection-id}
> Collection by ID


#### Path parameters

##### &#9655; id

UUID of the collection


<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>In</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>id  <strong>(required)</strong></td>
        <td>
          string
        </td>
        <td>path</td>
        <td>UUID of the collection</td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>








#### Responses



##### ▶ 200 - Successful operation

###### Headers
_No headers specified_


##### ▶ 404 - Request Parsing Error

###### Headers
_No headers specified_


#### Tags

<div class="tags">
  <div class="tags__tag"></div>
</div>
</div>

### `GET` /collection/{id} #{op-get-collection-id}
> Collection by ID


#### Path parameters

##### &#9655; id

UUID of the collection


<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>In</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>id  <strong>(required)</strong></td>
        <td>
          string
        </td>
        <td>path</td>
        <td>UUID of the collection</td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>








#### Responses



##### ▶ 200 - Successful operation

###### Headers
_No headers specified_

###### application/json


[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>meta</td>
        <td>
          object
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>meta.totalGranules</td>
        <td>
          integer
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>data</td>
        <td>
          array
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>


##### Example _(generated)_

```json
{
  "meta": {
    "totalGranules": 0
  },
  "data": [
    {
      "type": "collection",
      "id": "string"
    }
  ]
}
```

##### ▶ 404 - Request Parsing Error

###### Headers
_No headers specified_


#### Tags

<div class="tags">
  <div class="tags__tag"></div>
</div>
</div>

### `POST` /search/collection #{op-post-search-collection}
> Retrieve collection metadata

Retrieve collection metadata records matching the text query string, spatial, and/or temporal filter.





#### Request body
[object Object]

###### application/json



[Search Request](schema/request.md)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>queries</td>
        <td>
          array
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>filters</td>
        <td>
          array
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>facets</td>
        <td>
          boolean
        </td>
        <td>Flag to request counts of results by GCMD keywords in addition to results. Defaults to false if not provided.</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>summary</td>
        <td>
          boolean
        </td>
        <td>Flag to request summary of search results instead of full set of attributes. Defaults to true if not provided.</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>page</td>
        <td>
          object
        </td>
        <td>Pagination of results</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>page.max <strong>(required)</strong></td>
        <td>
          integer
        </td>
        <td>Maximum number of results returned. If the page object is not provided, this defaults to 10.</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>page.offset <strong>(required)</strong></td>
        <td>
          integer
        </td>
        <td>Number of records by which to offset results. If the page object is not provided, this defaults to 0.</td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>


##### Example

> basic text query



```json
{
  "queries": [
    {
      "type": "queryText",
      "value": "climate"
    }
  ],
  "filters": [],
  "facets": true,
  "page": {
    "max": 20,
    "offset": 0
  }
}
```

##### Example

> multiple science theme filters selected



```json
{
  "queries": [
    {
      "type": "queryText",
      "value": "weather"
    }
  ],
  "filters": [
    {
      "type": "facet",
      "name": "science",
      "values": [
        "Agriculture",
        "Atmosphere > Atmospheric Radiation > Incoming Solar Radiation"
      ]
    }
  ],
  "facets": true,
  "page": {
    "max": 20,
    "offset": 0
  }
}
```

##### Example

> multiple facets selected



```json
{
  "queries": [
    {
      "type": "queryText",
      "value": "weather"
    }
  ],
  "filters": [
    {
      "type": "facet",
      "name": "science",
      "values": [
        "Agriculture"
      ]
    },
    {
      "type": "facet",
      "name": "instruments",
      "values": [
        "ADCP > Acoustic Doppler Current Profiler"
      ]
    }
  ],
  "facets": true,
  "page": {
    "max": 20,
    "offset": 0
  }
}
```

##### Example

> Next Page request



```json
{
  "queries": [
    {
      "type": "queryText",
      "value": "weather"
    }
  ],
  "filters": [],
  "facets": false,
  "page": {
    "max": 20,
    "offset": 20
  }
}
```




#### Responses



##### ▶ 200 - Successful operation

###### Headers
_No headers specified_

###### application/json


[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>meta</td>
        <td>
          object
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>meta.took</td>
        <td>
          integer
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>meta.total</td>
        <td>
          integer
        </td>
        <td>total number of results matching the search</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>meta.facets</td>
        <td>
          object
        </td>
        <td>included if search request specified facets:true</td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>data</td>
        <td>
          array
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>


##### Example _(generated)_

```json
{
  "meta": {
    "took": 0,
    "total": 0,
    "facets": {}
  },
  "data": [
    {
      "type": "collection",
      "id": "string",
      "attributes": {
        "title": "string",
        "thumbnail": "http://example.com",
        "beginYear": "2019-02-15",
        "endYear": "2019-02-15",
        "spatialBounding": {
          "type": "Point",
          "coordinates": [
            -360,
            -90
          ]
        },
        "links": [
          {
            "linkProtocol": "string",
            "linkFunction": "string",
            "linkDescription": "string",
            "linkUrl": "http://example.com",
            "linkName": "string"
          }
        ]
      }
    }
  ]
}
```

##### ▶ 400 - Bad Request

###### Headers
_No headers specified_


#### Tags

<div class="tags">
  <div class="tags__tag"></div>
</div>
</div>

## Schemas


#### fullCollectionResponse

[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>meta</td>
        <td>
          object
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>meta.totalGranules</td>
        <td>
          integer
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
      <tr>
        <td>data</td>
        <td>
          array
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>

##### Example _(generated)_

```json
{
  "meta": {
    "totalGranules": 0
  },
  "data": [
    {
      "type": "collection",
      "id": "string"
    }
  ]
}
```

#### collectionMetadataObject

[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>totalGranules</td>
        <td>
          integer
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>

##### Example _(generated)_

```json
{
  "totalGranules": 0
}
```

#### collectionDataObject

[](.)

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Accepted values</th>
    </tr>
  </thead>
  <tbody>
      <tr>
        <td>type</td>
        <td>
          string
        </td>
        <td></td>
        <td><code>collection</code></td>
      </tr>
      <tr>
        <td>id</td>
        <td>
          string
        </td>
        <td></td>
        <td><em>Any</em></td>
      </tr>
  </tbody>
</table>

##### Example _(generated)_

```json
{
  "type": "collection",
  "id": "string"
}
```
