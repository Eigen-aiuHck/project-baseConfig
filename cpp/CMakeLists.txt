cmake_minimum_required(VERSION 3.16)

set(PROJECT_NAME projectConfig)
set(BUILD_OUTPUT_NAME main_app)

project(${PROJECT_NAME}
	VERSION 0.0.1
	DESCRIPTION "Configure template project"
	LANGUAGES CXX)

add_executable(${BUILD_OUTPUT_NAME} ${CMAKE_CURRENT_SOURCE_DIR}/src/main.cpp)
target_compile_features(${BUILD_OUTPUT_NAME} PUBLIC cxx_std_17)
target_compile_options(${BUILD_OUTPUT_NAME} PUBLIC
	$<$<CXX_COMPILER_ID:Clang>:
		$<$<CONFIG:Debug>:-g -O0 -Wall>
		$<$<CONFIG:Release>:-O3 -Wall>
		$<$<CONFIG:RelWithDebgInfo>:-g -O3 -Wall>
	>
)
target_include_directories(${BUILD_OUTPUT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
