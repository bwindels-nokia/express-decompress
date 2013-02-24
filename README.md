Supports gzip and deflate compression. Add this middleware before the body parser in order to have request.body populated as normal with compressed requests:

```
app.use(require('express-decompress').create());
...
app.use(express.bodyParser());
```

Supports gzip and deflate compression.