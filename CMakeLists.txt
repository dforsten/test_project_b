cmake_minimum_required(VERSION 3.6)

project(test-project-b
	VERSION 1.0.0
	LANGUAGES CXX
	DESCRIPTION "Test Project B."
	)

include(GNUInstallDirs)
install(DIRECTORY include/ CONFIGURATIONS Release DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}/test-project-b" FILES_MATCHING PATTERN "*")
