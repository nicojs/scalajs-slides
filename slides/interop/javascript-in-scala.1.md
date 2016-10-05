* Using Type Fascade

```scala
// JQuery.scala
@js.native
trait JQueryStatic extends js.Object {
  def apply(selector: String): JQuery = js.native
}
@js.native
trait JQuery extends js.Object {
 def html(htmlString: String): JQuery = js.native
 // ...
}
```
```scala
// MyApp.scala
import org.scalajs.jquery.jQuery

object MyApp{
  val jQuery: JQueryStatic = js.Dynamic.global.
    jQuery.asInstanceOf[JQueryStatic]

  jQuery(".h1").html("hello world")
}
```
