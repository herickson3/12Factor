Configuration

note:
Never have code that branches based on where it's running

Static values can come from the environment, and dynamic data from backing services


Bad
```javascript
var host = getHostName()

var db

if ( host == "dev-server:3000" ) {
  db = newDBConnection(devConfig)
}

if ( host == "prod-server.com" ) {
  db = newDBConnection(prodConfig)
}
```

Good
```javascript
var dbConfig = environment.getVar('DB_CONFIG')

var db = newDBConnection(dbConfig)
```
