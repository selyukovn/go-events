## [0.3.0] - 2026-02-25

### BREAKING CHANGES

In `v0.2.1` the project was renamed, so the import paths were changed too.
This was not mentioned as a `breaking change` and was incorrectly tagged as a bugfix.

*Note: v0.2.1 has been retracted.*

---

## [0.2.1] - 2026-02-24

Project renamed from `go-event-dispatcher` to `go-events`.

---

## [0.2.0] - 2025-11-23

### BREAKING CHANGES

- Default `Dispatcher` implementation replaced with more simple `DispatcherImplGeneralFn`.

---

## [0.1.0] - 2025-11-06

### FEATURES
- Added basic abstractions `DispatcherInterface` and `EventInterface`.
- Added `Dispatcher` as default implementation of the dispatcher interface.\
  Handlers are resolved via user‑supplied function at dispatcher creation. 
- Added `Event` struct with `OccurredAt() time.Time` method to avoid boilerplate in custom events.
- Added `Collection` for accumulating events before processing.\
  Implemented pre-allocation ability via `ColOptInitialSize(int)` and ability to work in async mode via `ColOptAsync()`.
- Basic tests for `Dispatcher` and `Collection`.
