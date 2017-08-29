Think of your app as a pure function

note:
any state only exists under the context of a single request

assume that your app is started up and shut down for every request

following the previous suggestions helps achieve this.


Bad
```javascript
var myState = files.read('state-file.json')

function myApp(request) {
  myState.update(newData)
  
  return response
}
```

Good
```javascript
function myApp(request) {
  var myState = backingService.read()

  // process request
  // update state

  backingService.write(myState)

  return response
}
```
