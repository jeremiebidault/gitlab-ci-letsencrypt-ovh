## generate API creds for OVH

#### useful links

access API interface

```https://eu.api.ovh.com/console/```

get applications list

```https://api.ovh.com/console/#/me/api/```

create API token

```https://eu.api.ovh.com/createToken/```

#### API access

Get this object properties

```GET /domain/zone/```

Zone status (payload : isDeployed, errors, warnings)

```GET /domain/zone/domain.tld/status```

Records of the zone (payload: records list of IDs)

```GET /domain/zone/domain.tld/record```

Get this object properties (payload : record details)

```GET /domain/zone/domain.tld/record/*```

Create a new DNS record (Don't forget to refresh the zone)

```POST /domain/zone/domain.tld/record```

Apply zone modification on DNS servers (payload : bollean)

```POST /domain/zone/domain.tld/refresh```

Delete a DNS record (Don't forget to refresh the zone)

```DELETE /domain/zone/domain.tld/record/*```
