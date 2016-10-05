## Undefined behavior

Not-implemented and therefore considered *undefined behavior*:

<small>NullPointerException, ArrayIndexOutOfBoundsException, StringIndexOutOfBoundsException, ClassCastException, ArithmeticException, StackOverflowError, other VirtualMachineErrors</small>

Configure the `ClassCastException` to be JVM *compliant*:

```scala
scalaJSSemantics ~= { _.withAsInstanceOfs(
  org.scalajs.core.tools.sem.CheckedBehavior.Compliant) }
```
