# learning-full-stack-javascript-development
[Learning Full-Stack JavaScript Development: MongoDB, Node, and React](https://www.linkedin.com/learning/learning-full-stack-javascript-development-mongodb-node-and-react/modern-javascript)

### HTTP/HTTPS Modules
This pulls in status code then html from page.
Test in console with
babel-node server.js | less
```
import https from 'https'

https.request(...)

  https.get('https://www.lynda.com', res => {
    console.log('Response status code: ', res.statusCode)
    res.on('data', chunk => {
      console.log(chunk.toString())
    })
  })

```
