Superpromise
=============
> wrap superagent requests in promises

**example:**

``` js
const sa= require('superagent');
const sp = require('superpromise');

const request = sa.get('http://www.duckduckgo.com');
sp(request).then(function(res){
  // success
}).catch(function(err) {
  // failure
});
```
