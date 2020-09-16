# Functional programming

We have seen that functions are easier to understand and use. They have clear inputs and return clear output. Because they are easier to understand, they are also easier to change in future.

## Few tips when writing functions

### Avoid global variables

```js
var url = '/api/'

function handleUpload (data, callback) {
    ajax(url, data, callback)
    setStatus('uploading...')
}
```

The `handleUpload` function is using an outside variable `url`. One cannot use this function without understanding the outside code too.

The value of `url` can be change inside code. Thus calling `handleUpload` with exact same inputs can give different outcomes. And due to this, we must be aware of the value of `url` when we write or use `handleUpload` function.


Compare the above function with this:

```js
function handleUpload (url, data, callback) {
    ajax(url, data, callback)
    setStatus('uploading...')
}
```

We can write `handleUpload` function much more clearly because we have all the variable inputs defined. We don't need to be aware of any outside variable to write it or use it. This will be much more predictable function.
