# fake-api
Fake API using my-json-server.typicode.com

## Resources

- https://my-json-server.typicode.com

## Usage

GET all users:

```
$ curl https://my-json-server.typicode.com/ruanbekker/fake-api/users

[
  {
    "id": 1,
    "country": "south africa",
    "city": "cape town",
    "name": "ruan"
  }
]
```

GET a user:

```
$ curl https://my-json-server.typicode.com/ruanbekker/fake-api/users/1
{
  "id": 1,
  "country": "south africa",
  "city": "cape town",
  "name": "ruan"
}
```

POST on users (no persistence):

```
$ curl -XPOST -H 'Content-Type: application/json' https://my-json-server.typicode.com/ruanbekker/fake-api/users -d '
{"country": "kenya", "city": "nairobi", "name": "james"}'

{
  "country": "kenya",
  "city": "nairobi",
  "name": "james",
  "id": 2
}
```
