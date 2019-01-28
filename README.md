# Goodreads Graphql API

## Queries

```
{
  author(id: 23) {
    name,
    books {
      title,
      isbn
    }
  }
}
```
```
{
  author(id: 23) {
    name,
    books {
      title,
      isbn,
      authors {
        name
      }
    }
  }
}
```

```
{
  author(id: 23) {
    name,
    books {
      title,
      isbn,
      authors {
        name,
        books {
          title,
          authors {
            name
          }
        }
      }
    }
  }
}
```