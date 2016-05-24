Super Promise
=============
> wrap super agent requests in promises

**example:**

``` js
const superagent = require('superagent');
const sp = require('superpromise');

const request = superagent.get('http://www.google.com');
sp(request).then(function(res){
  // success
}).catch(function(err) {
  // failure
});
```
