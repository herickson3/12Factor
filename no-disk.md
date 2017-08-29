Don't write to disk

note:
assume you don't have a disk

if your app needs a disk, it's no longer an app it's a machine

any persistent data can be written to a service, even files

DB, Cache, S3


Bad

```javascript
file = open( 'myCache.json' )

var newData = update( file.data, {some: "newData"} )

file.write( newData )
```

Good

```javascript
oldData = s3.get( 'some-bucket/myCache.json' )

var newData = update( oldData, {some: "newData"} )

s3.write( 'some-bucket/myCache.json', newData )
```
