Think of your app as a function

note:
any state only exists under the context of a single request

assume that your app is started up and shut down for every request

following the previous suggestions helps achieve this



```go
func myApp(request http.Request) http.Response {
  var correctResponse http.Response
  // process request
  return correctResponse
}
```


