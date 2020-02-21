#----------
# Main-Application
#----------

project(Main LANGUAGES CXX)

# Add an executable target to the project
add_executable(${PROJECT_NAME} main.cpp)

# Specify local libraries to use when linking
target_link_libraries(${PROJECT_NAME}
  PRIVATE
    lib::Hello
    lib::PocoTimer
)
