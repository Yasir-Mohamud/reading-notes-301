# APIs
__________

- SuperAgent is a ajax API made for flexibility ,low learning curve and readability.It works with Node.js.

- a basic request looks like this 

``` js 
request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
   ```
- 

# GET REQUEST 
______________

- Use the query.() method which makes a string and accepts string as arguments.
``` js

request
    .get('/querystring')
    .query('search=Manny&range=1..5')
    .then(res => {

    });


```

# HEADER REQUEST 
_________________

- Also uses the query.() method.
``` js

request
    .head('/user')
     .query({ email: 'joe@smith.com' })
    .then(res => {

    });


```

# CORS
_________

- withCredentials() method enables sending of cookies from the origin only when Access-Control-Allow-Credentials is "true".

``` js 
request
  .get('https://api.example.com:4001/')
  .withCredentials()
  .then(res => {
    assert.equal(200, res.status);
    assert.equal('tobi', res.text);
  })
  ```

  