Aggregation, Graphing, and Historical Values
============================================

metrics-clojure is a wrapper around metrics, and metrics only stores the current
value of any given metric.  It doesn't keep the values at previous times around
(aside from the one/five/fifteen minute windows for timers and meters).

Not storing historical data is important because it allows metrics to be used in
production without worrying about memory usage growing out of control.

In practice you'll want to not only view these instantaneous values but also
their values over time.  For this you'll need to turn to external utilities.

You can implement a solution yourself as we'll show in the example below, or use
an existing utility that metrics-clojure provides support for.

Sending Metrics to Graphite
---------------------------

**TODO**

Sending Metrics to Ganglia
--------------------------

**TODO**

Implementing a Simple Graphing Server
-------------------------------------

**TODO**
