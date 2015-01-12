# cmake-tests

Some CMake edge case tests.

 * file\_rel: file(RELATIVE\_PATH ...) test. Looks like it can't handle pats
   with dots properly.
 * set\_parent: set(VAR "" PARENT\_SCOPE) seems not working. It leaves variable
   unset (compare it to set(VAR "") in current scope)
