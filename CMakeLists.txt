add_library(sqlite SHARED sqlite3.c)
target_compile_definitions(
  sqlite PRIVATE 
  "SQLITE_ENABLE_MATH_FUNCTIONS"
)
set_property(
  TARGET sqlite PROPERTY POSITION_INDEPENDENT_CODE ON
)
