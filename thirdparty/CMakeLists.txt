subdirs(glfw KTX-Software)

set(TARGET_NAME imgui)
add_library(
  ${TARGET_NAME}
  imgui/imgui.cpp
  imgui/imgui_draw.cpp
  imgui/imgui_widgets.cpp
  imgui/imgui_tables.cpp
  imgui/imgui_demo.cpp
  imgui/backends/imgui_impl_glfw.cpp
  imgui/backends/imgui_impl_opengl3.cpp)
target_include_directories(
  ${TARGET_NAME} PUBLIC ${CMAKE_CURRENT_LIST_DIR}/imgui
                        ${CMAKE_CURRENT_LIST_DIR}/imgui/backends)
target_link_libraries(${TARGET_NAME} PRIVATE glfw)
