## Reflection

No reflection support other than limited `java.lang.Class` support

```scala
val nicojs = Person("NicoJS", 30, PrisonBreak)

println(nicojs.getClass.getName)
// OK: tutorial.webapp.People$Person

nicojs.getClass.getMethod("name").invoke(nicojs)
// [error] Referring to non-existent method
// java.lang.Class.getMethod(
//    java.lang.String,[java.lang.Class)java.lang.reflect.Method
```
