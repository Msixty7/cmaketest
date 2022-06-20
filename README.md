# cmaketest
A minimal cmake sample project to demonstrate a problem in cmake.

Cmake will not find a CXX compiler if the path to Xcode or the Xcode application name contains a SPACE.

# Error output:
´´´cmake
-- The C compiler identification is AppleClang 13.1.6.13160021
-- The CXX compiler identification is AppleClang 13.1.6.13160021
CMake Error at CMakeLists.txt:3 (project):
  No CMAKE_C_COMPILER could be found.



CMake Error at CMakeLists.txt:3 (project):
  No CMAKE_CXX_COMPILER could be found.



-- Configuring incomplete, errors occurred!
See also "..../cmaketest_build/CMakeFiles/CMakeOutput.log".
´´´
