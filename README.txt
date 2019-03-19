
# Notes about Nodejs

## Best Practices 

All method that are asyncronous must have a callback parameter

The callback parameter must be the last one

The first callback argument must be "err", with null value if no error

Each callback must start with if(err)

```
function callback(err,values) {

	if(err) {
		console.log(err);
		return;
	}

}
```



