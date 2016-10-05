## Call JavaScript from Scala

```JavaScript
// a-file.js
var jQuery = function(/*...*/){
    // ...
};
```

* Using Dynamic

```scala
// app.scala
import scala.scalajs.js

object App {
    js.Dynamic.global.jQuery(".h1").html("hello world")
}
```


