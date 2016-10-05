## Call Scala from JavaScript

* Using annotations

```scala
// Square.scala
import org.scalajs.dom.html

@JSExport
object Square {

  @JSExport
  def draw(canvas: html.Canvas): Unit = {
  }
}
```

```js
// a-file.js
Square().draw(document.createElement('canvas'));
```
