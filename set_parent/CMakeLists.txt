cmake_minimum_required(VERSION 2.8)

function (test_parent _var)
    set("${_var}" "" PARENT_SCOPE)
endfunction ()

set(test_var)
test_parent(test_var)

if (DEFINED test_var)
    message("Test passed")
else ()
    message(FATAL_ERROR "Test failed")
endif ()
