file(GLOB LIB . *.c)

add_library(lib ${LIB})

add_test(NAME TestCarre COMMAND calculator car 5)

set_tests_properties(TestCarre PROPERTIES PASS_REGULAR_EXPRESSION "25")
