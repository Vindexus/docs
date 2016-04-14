# Connect API (Alpha)

Write Date: April 14, 2016
API Version Prefix: `/api`

## Routes

### GET `/catalog/track` 

Gets all tracks. You can use default collection query options.

**WARNING**
> Even though this route is publicly available it may not be available in future releases.
> It is advised to fetch releases and their tracks. See below.

### GET `/catalog/track/:id` 

Gets a track by id.

### GET `/catalog/release` 

Gets all releases. You can use default collection query options.

### GET `/catalog/release/:id` 

Gets a release by id.

### GET `/catalog/release/:id/tracks` 

Gets you tracks for a release. You can use default collection query options.

### GET `/playlist` 

Gets you a playlist that is publicly available.

### GET `/playlist/:id/tracks` 

Gets you tracks for a playlist. You can use default collection query options.

## Query Options

Query options are simple URL query string key values.

### Collections

#### Fields 

`fields=a,b,c`

Specifiy what fields you wish to recieve by a comma separated string.

**WARNING**
> Some fields are manatory and will appear anyways.

#### Identifiers 

`ids=id1,id2`

Specifies specific ids you want to fetch instead of the whole collection.

#### Offset/Skip 

`skip=100`

Specifies the starting point of the collection you wish to fetch.

#### Amount/Limit 

`limit=10`

Specifies the number of results you wish to fetch.

**WARNING**
> In the future it may be capped.

#### Filter/On 

`by_key=akey&by_value=avalue`

Filters on the specified key for the value.

**WARNING**
> To be replaced with a more abstract technique.
