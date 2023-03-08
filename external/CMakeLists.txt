

add_subdirectory(Vulkan-Headers)
add_subdirectory(Vulkan-Loader)

set(VMA_STATIC_VULKAN_FUNCTIONS ON)
set(VMA_DYNAMIC_VULKAN_FUNCTIONS OFF)
add_subdirectory(VulkanMemoryAllocator)

option(GLFW_BUILD_EXAMPLES OFF)
option(GLFW_BUILD_TESTS OFF)
option(GLFW_BUILD_DOCS OFF)
add_subdirectory(glfw)

add_subdirectory(glm)

add_subdirectory(freetype)


set(BUILD_SHARED_LIBS ON)
set(IL_TESTS OFF)
add_subdirectory(DevIL/DevIL/src-IL)
add_subdirectory(DevIL/DevIL/src-ILU)
set(BUILD_SHARED_LIBS OFF)
