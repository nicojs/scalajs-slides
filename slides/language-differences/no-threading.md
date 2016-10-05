## No multi threading

* JavaScript is single threaded
* You *can* make use of futures for async work
    * Gets translated as promises
    * Execution context: `scala.scalajs.concurrent.JSExecutionContext`
        * `runNow`: Run sync
        * `queue`: Run in next microtask
* Limitations on using `Await`
