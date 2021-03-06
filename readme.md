# GraphQL with NodeJs

Simple web app to search for movies and directors

## Getting Started


### Prerequisites

What things you need to install

```
npm
```

### Installing

```
npm install
```

### Running

```
node server.js
```

## Requests

Get movie name by id

```
{
  movie(id: 1) {
    name
  }
}
```

Get movies for id with some fields

```
{
  movie(id: 3) {
    name
    id
    year
  }
}
```

Get director by id

```
{
  director(id: 1) {
    name
    id,
    age
  }
}
```
(More complex) Get director by id with fields and his movie with some fields

```
{
  director(id: 1) {
    name
    id,
    age,
    movies{
      name,
      year
    }
  }
}
```