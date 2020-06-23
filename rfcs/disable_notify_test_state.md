# RFC ??: Add a new test property to not displaying test state

## Summary

Add a new test property called `notify_test_state` to not displaying
test state when tests are running.

## Details

In testharness there are a few usage of `notify_test_state` function,
which outputs the test state to the documents during test
runs. Some tests are sensitive to the content of the documents,
so the test state output may interfere the test results.

We are adding a new setup property to prevent outputting the
test state.

## Risks

No risks as this is an opt-in property.
