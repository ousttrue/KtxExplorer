set(TARGET_NAME KtxExplorer)
add_executable(${TARGET_NAME} main.cpp)
target_link_libraries(${TARGET_NAME} PRIVATE imgui glfw OpenGL32)
