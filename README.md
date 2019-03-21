
# Notes about JS & Nodejs

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

	... do some stuff with values
}
```
## Ecmascript

Use a compiler to code using latest ECMAScript standard

Replace Anonymous function by ([var]) => {}, it will scope this to the caller and not the anonymous function. 
Replacing the var myself = this;

Define Key and Value of object, with only one variable name : {foo} <=> {foo:foo}

ALWAYS use await when function is Promise compatible

If function is not Promise compatible, create a Promise to wrap it in an async function

## NodeJS

Use __dirname and __filename magic global to deals about current file


## Express

Always declare middleware app.use before declaring the route itself

