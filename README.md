Repro for https://github.com/ChilliCream/graphql-platform/issues/3682


In order to run this demo start the following redis docker container:


```bash
docker run --name redis-stitching -p 7000:6379 -d redis
```

Use this query

```graphql
query me {
  me {
    reviews2 {
      id
    }
  }
}
```