# threads.h
Cross platform thread macros for C.

## Caveats

`MUTEX_TRY_LOCK()` and `PMUTEX_TRY_LOCK()` return true if acquired locked, otherwise false.

`THREAD_CREATE()` return 0 on success, otherwise non-zero.

`threadPriority{In,De}crease()` return false on success, otherwise true.

## Changes

```
August 2, 2018      "1.4" Added priority and THREADS_WIN_XP_FTW.
June 13, 2018       "1.3" Added "do{}while" because really I should of done this forever ago. Added error checking.
January 22, 2013    "1.2" typedefed THREAD (for IDE color)
January 19, 2012    "1.1" Added getNumCores()
May 26?, 2011       "1.0" Added MUTEX_TRY_LOCK and PMUTEX_TRY_LOCK
January 31?, 2011   Unreleased? initial version
```
