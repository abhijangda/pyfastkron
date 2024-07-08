add_subdirectory(pybind11)
add_subdirectory(fastkron)
pybind11_add_module(PyFastKronWrapper ${CMAKE_CURRENT_SOURCE_DIR}/src/pywrapper.cpp)
target_link_libraries(PyFastKronWrapper PRIVATE FastKron)