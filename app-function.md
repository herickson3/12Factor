Think of your app as a pure function

note:
any state only exists under the context of a single request

assume that your app is started up and shut down for every request

following the previous suggestions helps achieve this



```javascript
function myApp(request) {
  // process request
  return correctResponse
}
```
