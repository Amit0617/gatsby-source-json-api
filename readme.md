Pull data from a JSON API endpoint and turn into Gatsby nodes

#### Install
```
npm i git+https://github.com/amit0617/github-source-json-api
```

#### Usage
```js
plugins: [
  resolve: 'gatsby-source-json-api',
  options: {
    // name the gatsby node
    name: 'SwaggerAPI',
    // url for JSON endpoint
    uri: 'www.example.com/example.json',
    // Basic Auth if required (optional)
    auth: {
      username: 'userename',
      password: 'password'
    },
    // Custom header if required (optional)
    header: {
    "X-Custom-Header": "identifier_value"
    },
    // image location to process images. Default: "image.url"
    image_location: "image.url",
  }
]
```
