======================
streamz_ext Change Log
======================

.. current developments

v0.2.1
====================

**Added:**

* Tools for linking pipeline chunks together
* ``zip`` and ``zip_latest`` take in ``first`` kwarg so that those nodes can
  be run first (rewriting the execution graph order)




v0.2.0
====================

**Added:**

* ``first`` kwarg to ``combine_latest`` allowing users to re-order the pipeline
  as needed when using ``combine_latest``. This helps with jug handle like
  graphs where a source node is both part of both the incoming streams, by
  allowing the ``emit_on`` stream(s) to be computed later, permitting the
  buffers to be filled when ``emit_on`` emits.
* Test for ``unique`` using lists




v0.1.0
====================

**Added:**

* ``orch`` build system


**Changed:**

* ``unique`` now handles all non hashables in a ``deque`` rather than just
  ``dict``s
* Pull tests from streamz


**Removed:**

* Most of the defined nodes, as ``streamz`` has caught up to us.




v0.0.2
====================

**Added:**

* Args and kwargs to the filter node

* Imports from all the streamz tests for more coverage

* Conda-forge activity to rever




v0.0.1
====================

**Added:**

* Add rever
* Initialize project for extending mrocklin/streamz




