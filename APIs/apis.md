# APIs

## What are APIs?

- Application Programming Interface
- A simple interface for complex action
- A URL makes a request to a server, the server will handle the request and respond. The response is oftentimes formatted in JSON

## Syntax

```js
fetch(url)
  .then((res) => res.json()) //parse response as json
  .then((data) => {
    console.log(data);
  })
  .catch((err) => {
    console.log(`error ${err}`);
  });
```
